# Project Header, Hero & Cards

For Rocket Emoji 🚀 -> https://emojipedia.org/

For Hamburger Icon &#9776; -> https://www.fileformat.info/info/unicode/char/2630/index.htm

A single-page marketing site for "Acme Rockets," built with semantic HTML and styled using [Tailwind CSS](https://tailwindcss.com/). It includes a sticky header with navigation, a hero section, a rocket product showcase, and placeholder sections for testimonials and contact info. The layout is responsive and supports both light and dark mode.

## Project Structure

```
.
├── index.html          # Main page (this file)
├── output.css          # Compiled Tailwind CSS (referenced via <link>)
└── images/
    ├── rocketdab.png
    ├── rocketman.png
    ├── rocketride.png
    └── rocketlaunch.png
```

> Note: `output.css` and the `images/` folder are referenced by the HTML but aren't included here — add your own assets or update the paths to match your project.

## Features

- **Sticky header** with a logo/brand link and a nav menu (Our Rockets, Testimonials, Contact Us)
- **Mobile menu button** (`#mobile-open-button`) — currently a static `☰` icon; hook up JS to toggle a mobile nav menu
- **Hero section** with headline, subtext, and a hero image
- **Rocket showcase** — three product cards (Explorer, Adventurer, Infinity) with responsive pricing/description text
- **Dark mode support** via Tailwind's `dark:` classes
- **Smooth-scroll anchor links** (`scroll-mt-*`) for in-page navigation
- **Testimonials** and **Contact Us** sections scaffolded but empty — ready for content

## Getting Started

1. **Add Tailwind CSS.** This page expects a compiled `output.css` next to it. If you're using the Tailwind CLI:
   ```bash
   npx tailwindcss -i ./input.css -o ./output.css --watch
   ```
2. **Add images.** Place `rocketdab.png`, `rocketman.png`, `rocketride.png`, and `rocketlaunch.png` inside an `images/` folder, or update the `src` attributes to point to your own assets.
3. **Open `index.html`** in a browser, or serve it locally:
   ```bash
   npx serve .
   ```

## Known Issues / TODO

- Duplicate `id="rockets"` is used on two elements (the `<section>` wrapping the rocket cards and the `<h2>` inside it) — IDs must be unique; consider renaming one (e.g. `id="rockets-section"`).
- The "Testimonials" and "Contact Us" `<section>` elements also reuse `id="rockets"` — update these to unique, descriptive IDs.
- `#mobile-open-button` has no attached behavior yet — add a script to toggle the mobile nav on click.
- Testimonials and Contact sections need content (currently just headings).

## Tech Stack

- HTML5
- Tailwind CSS (utility classes; dark mode via `dark:` variant)

## License

Add your preferred license here (e.g. MIT).