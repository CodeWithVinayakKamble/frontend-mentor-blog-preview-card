# Frontend Mentor - Blog preview card

### Built with

- Semantic HTML5 markup
- CSS custom properties (Variables)
- Flexbox
- BEM (Block Element Modifier) Naming Convention
- Fluid Typography & Layouts (using CSS `clamp()`)
- Mobile-first workflow

### What I learned

During this project, I really focused on writing strict, semantic HTML and mastering modern CSS techniques. Here are my biggest takeaways:

**1. Strict Accessibility:**
I learned that decorative images (like an avatar sitting right next to an author's name) should use an empty `alt=""` tag. This prevents screen readers from redundantly announcing the image name, creating a much better user experience.

**2. Fluid Layouts without Media Queries:**
Instead of writing multiple `@media` queries for different screen sizes, I learned how to use the `clamp()` function. This allowed me to set a flexible, dynamic width for my card that seamlessly adapts to any device:

```css
.preview-card {
  /* Be at least 280px, ideally 90% of the screen, but never more than 320px */
  width: clamp(17.5rem, 90%, 20rem);
}
```

**3. Advanced Semantic HTML:**
Instead of relying on generic `<div>` tags, I utilized semantic tags like `<article>` and `<time>`. I also learned that you can use a `<footer>` inside an `<article>` to hold metadata like author information!

**4. Flexbox Cross-Axis Quirks:**
I discovered that setting `align-items: center` on a column Flexbox stops the child elements from stretching across the screen. Removing it from the `body` allowed my main container to stretch properly while still staying centered.

### AI Collaboration

I worked with an AI Mentor to complete this challenge. Instead of writing code for me, the AI guided me through strict code reviews and helped me understand:
- The nuances of accessibility and screen reader behavior.
- How to structure my CSS variables and reset properly.
- The difference between `align-self: flex-start` and `width: fit-content` when dealing with Flexbox items.

## Author
- Challenge by Frontend Mentor Coded by Vinayak Kamble.