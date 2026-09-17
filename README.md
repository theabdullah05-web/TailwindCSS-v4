# Learning Tailwind CSS v4

This repo is my personal learning space for **Tailwind CSS v4** — notes, small exercises, and mini-projects as I go from the basics to more advanced patterns.

## Why v4?

Tailwind v4 is a big shift from v3: the engine was rewritten (the "Oxide" engine, built on Rust/Lightning CSS), and configuration moved from `tailwind.config.js` into CSS itself using `@theme`. There's no config file by default, builds are much faster, and content detection is automatic. This repo tracks what I'm learning as I adapt to these changes.

## Setup

This project uses the Vite plugin for Tailwind v4:

```bash
npm install tailwindcss @tailwindcss/vite
```

`vite.config.js`:

```js
import tailwindcss from '@tailwindcss/vite'

export default {
  plugins: [tailwindcss()],
}
```

`src/style.css`:

```css
@import "tailwindcss";

@theme {
  --color-brand-500: oklch(0.6 0.2 260);
  --font-display: "Inter", sans-serif;
}
```

## Running locally

```bash
npm install
npm run dev
```

## Topics I'm covering

- [ ] Utility-first fundamentals (spacing, flex, grid, typography)
- [ ] Responsive design & variants
- [ ] CSS-first theming with `@theme`
- [ ] Container queries
- [ ] Dark mode
- [ ] Reusable components with `@apply` / component patterns
- [ ] Migrating mental models from v3 → v4

## License

MIT (or update as you prefer)
