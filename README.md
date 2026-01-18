<!-- Use Ctrl/Cmd + Shift + V in VS Code to preview this Markdown file. -->

# Project Challenge #1: Testimonial Card

---

## **Tech Stack and Approach**

I approached this challenge using **vanilla HTML and CSS** to focus on semantic markup and flexbox fundamentals. The layout uses a **flexbox-centered container** pattern where the `<main>` element handles vertical and horizontal centering of the testimonial card. I structured the HTML semantically with a `<main>` landmark for the primary content and a `<footer>` for attribution, keeping the markup minimal and accessible. For styling, I used **CSS custom properties** for consistent spacing and avoided frameworks to strengthen my understanding of core CSS concepts. The responsive design uses **media queries** to adjust padding and card width across mobile, tablet, and desktop breakpoints based on the design system specifications.

---

## **Useful Resources and Lessons Learnt**

**Resources:**
- [MDN Flexbox Guide](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox) 
- [CSS-Tricks Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) 
- [MDN HTML Semantics](https://developer.mozilla.org/en-US/docs/Glossary/Semantics#semantics_in_html)

**Key Lessons:**
- Using `min-height: 100vh` on both body and main ensures the layout fills the viewport properly
- Flexbox centering (`display: flex; align-items: center; justify-content: center`) is cleaner than margin-based approaches
- Keeping semantic HTML simple - not every component needs `<article>` or `<section>`, plain `<div>` is fine for structural elements
- `box-sizing: border-box` prevents padding from breaking layout calculations
---

## **Notes/Questions for Community**

**Questions:**
- **Semantic HTML best practices:** Should a single testimonial card use `<article>` since it's self-contained content, or is `<div>` sufficient for a simple UI component? I used `<div>` but would love feedback on this decision.
- **Class naming conventions:** I used simple names like `.testimonial-card` and `.profile` - are there any other naming methods I could follow? 
- **Accessibility considerations:** Beyond adding `alt` text to images, what other accessibility improvements should I consider? 
- **Container patterns:** Is it better to have the container handle all centering logic, or should cards be self-centering?

**Notes:**
- Initially struggled with `<main>` not filling the viewport - solved by setting `min-height: 100vh` on both `<body>` and `<main>`
- Chose flexbox over grid for centering since it's a single-item layout
- Used relative units (`rem`, `em`) for spacing to improve scalability and accessibility

