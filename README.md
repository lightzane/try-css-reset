# CSS Reset

Trying out how to do a minimum CSS Starter or **CSS reset** to get started with CSS on a blank project.

## Basic

[See reference](./src/styles/resets/basic.reset.css)

See also [preflight](./src/styles/resets/preflight.reset.css)

```css
*,
*::before,
*::after {
  box-sizing: border-box;
}

* {
  margin: 0;
  padding: 0;
  font: inherit;
}

ul[role='list'],
ol[role='list'] {
  list-style: none;
}

html:focus-within {
  scroll-behavior: smooth;
}

html,
body {
  height: 100%;
}

body {
  text-rendering: optimizeSpeed;
  line-height: 1.5rem;
}

a:not([class]) {
  text-decoration-skip-ink: auto;
}

img,
picture,
svg {
  max-width: 100%;
  display: block;
}

@media (prefers-reduced-motion: reduce) {
  html:focus-within {
    scroll-behavior: auto;
  }

  *,
  *::before,
  *::after {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
    scroll-behavior: auto !important;
  }
}
```

## Colors

```css
:root {
  --dracula-darker: hsl(231 15% 18%);
  --dracula-dark: hsl(232 14% 31%);
  --dracula-light: hsl(60 30% 96%);
  --dracula-blue: hsl(225 27% 51%);
  --dracula-cyan: hsl(191 97% 77%);
  --dracula-green: hsl(135 94% 65%);
  --dracula-orange: hsl(31 100% 71%);
  --dracula-pink: hsl(326 100% 74%);
  --dracula-purple: hsl(265 89% 78%);
  --dracula-red: hsl(0 100% 67%);
  --dracula-yellow: hsl(65 92% 76%);
}
```
