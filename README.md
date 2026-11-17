# Startpoint Pro — Single-File SaaS Landing Page

A dark, animated landing page for SaaS products and startups. Everything lives in one `index.html` file: HTML, CSS and JavaScript. No build step, no framework, no dependencies.

## What's in the pack

| File / folder | Purpose |
|---|---|
| `index.html` | The entire page (HTML, CSS, JavaScript) |
| `assets/` | Sample dashboard, phone, card and illustration images (replace with your own) |
| `README.md` | This guide |
| `LICENSE.txt` | Terms of use |

## Quick start

1. Unzip the pack.
2. Open `index.html` in a browser. It works offline except for the Inter font.
3. Replace the placeholder content (see the checklist below).
4. Upload the folder to any static host (Netlify, Vercel, GitHub Pages, cPanel, etc.).

## Features

- Hero with a 3D-tilting dashboard, floating badges and a cursor-following light
- Scroll progress bar, parallax background rings and staggered reveal animations
- Animations start only when their section scrolls into view (lazy initialisation)
- Feature cards with category filters and a cursor-tracking glow
- "How it works" cards you can interact with: a working create-project form, a task list and a calendar
- Count-up statistics
- Pricing cards with a monthly/yearly switch, a flip animation on prices and an animated border on the featured plan
- FAQ accordion, demo modal, toast messages, light and dark theme (remembered in the browser)
- Responsive layouts for desktop, tablet and phone, with a mobile menu
- Respects the visitor's "reduce motion" setting

## Replace before publishing (checklist)

- [ ] **Brand:** "Startpoint" in the `<title>`, the header, the hero, the footer and the copyright line
- [ ] **Hero text:** the title, the subtitle and the lead paragraph
- [ ] **Trust line:** the avatar initials and the "50,000+ teams" claim (only keep numbers you can back up)
- [ ] **Features:** the six `.feature` cards (icon, title, text, `data-category`)
- [ ] **Pricing:** the plan names, prices (`data-monthly` and `data-yearly` on each `.price`), features and buttons
- [ ] **Statistics:** the values in `data-count` and `data-suffix`
- [ ] **FAQ:** the questions and answers
- [ ] **Links:** the `href="#"` values in the footer and social icons; connect the "Start free trial" buttons to your sign-up page
- [ ] **Images:** replace everything in `assets/` with content you have the rights to use
- [ ] **Colors:** the variables at the top of the `<style>` block (`--cyan`, `--violet`, `--pink`, `--bg`)

The demo modal, plan buttons and CTA are demo-only: they show a message and do not take payment. Connect them to your own checkout or sign-up flow.

## Customization tips

- **Accent colors:** change the gradient colors in `.btn`, `.gradient` and the `:root` variables.
- **Animation strength:** adjust the tilt values in the script (`attachTilt(el, 8)`) and the durations in the CSS.
- **Remove a section:** delete its `<section>` block and its link in the header.
- **Reduced motion:** the page respects the visitor's setting automatically.

## Browser support

Current Chrome, Edge, Firefox and Safari on desktop and mobile. The 3D tilt and cursor effects are only active on devices with a mouse.

## Fonts

The page loads the Inter font from Google Fonts after the first paint (SIL Open Font License). If the font cannot load, the page falls back to the system font.

## Support

For help with setup or customization, contact: **[your email here]**
