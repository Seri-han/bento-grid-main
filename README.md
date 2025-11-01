# Frontend Mentor - Bento Grid Solution

![Design preview for the Bento grid coding challenge](./preview.jpg)

## 📖 Overview

This is my solution for the [Bento Grid challenge](https://www.frontendmentor.io/challenges/bento-grid-RMydElrlOj) on Frontend Mentor.  
The goal was to recreate the Bento-style layout using **only HTML and CSS**, focusing on **responsive grid design** and **clean structure**.

---

## 🎯 The challenge

Users should be able to:

- View the layout optimized for their device’s screen size (mobile, tablet, desktop)
- See a responsive and adaptive grid structure
- Experience clean visual hierarchy and balanced spacing

---

## 🧱 Built with

- Semantic **HTML5**
- **CSS Grid** for the layout
- **CSS custom properties (variables)** for theme consistency
- **Modern CSS features** such as `@layer`, logical properties, and `text-wrap: balance`
- **Locally hosted variable fonts** (DM Sans)

---

## 🧩 My process

1. **Setup**  
   Linked local fonts and structured the CSS into layers (`reset`, `base`, `layout`, `utilities`) for better organization.

2. **Layout**  
   Built a responsive grid using named areas.  
   The grid automatically reflows from single-column on mobile → two-column on tablet → full bento grid on desktop.

3. **Styling**  
   Applied a design token system using `--bento-card-*` custom properties to control padding, colors, and alignment per card.

4. **Fine-tuning**  
   Added responsive adjustments, overflow handling, and consistent border radius and spacing.

---

## 🧠 What I learned

- How to use **CSS Grid areas** dynamically across breakpoints.
- Leveraging **CSS custom properties** to style components without repeating code.
- Structuring large stylesheets using `@layer` for clarity and control over cascade.
- Working with **variable fonts** and optimizing layout responsiveness.

Example of my grid structure logic:

```css
@media (width > 960px) {
  .bento-grid {
    grid-template-areas:
      "seven one one four"
      "seven two three four"
      "eight two three four"
      "eight six five five";
  }
}

## Useful resources

MDN CSS Grid Guide
Josh Comeau’s CSS reset guide

## 🌐 Live Demo
🔗 [View the live site here](https://seri-han.github.io/bento-grid-main/)
🔗 [View the git code here](https://github.com/Seri-han/bento-grid-main)

## Author
Sarah Handal

## Acknowledgements

Thanks to Frontend Mentor for providing this challenge.
It was a great exercise in CSS architecture and layout precision.

## Feedback

I’d love your thoughts or suggestions on how to improve the structure or responsiveness.
Feel free to reach out or open an issue in the repo.