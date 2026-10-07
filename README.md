# Mattias Milger - Portfolio

[![Visit the site](https://img.shields.io/badge/Visit_the_site-mattiasmilger.github.io-2ecc71?style=for-the-badge)](https://mattiasmilger.github.io/)

My projects, all in one place.

---

A personal portfolio landing page that links to all of my projects, built with vanilla HTML, CSS, and JavaScript. Runs entirely client-side — no server or backend required. Designed for GitHub Pages.

**Run locally:** open `index.html` in any modern web browser. No build tools, compilers, or external dependencies required.

---

### Quick Links (Live Sites & Repositories)

- **Password Generator**: [Live App](https://mattiasmilger.github.io/Web-Password-Generator-by-Mattias/) | [GitHub](https://github.com/MattiasMilger/Web-Password-Generator-by-Mattias)
- **Image Editor**: [Live App](https://mattiasmilger.github.io/Web-Image-Editor-by-Mattias/) | [GitHub](https://github.com/MattiasMilger/Web-Image-Editor-by-Mattias)
- **Local Upload Server**: [GitHub](https://github.com/MattiasMilger/Local-Upload-Server)
- **Flashcards**: [Live App](https://mattiasmilger.github.io/Web-Flashcards-by-Mattias/) | [GitHub](https://github.com/MattiasMilger/Web-Flashcards-by-Mattias)
- **News Feed**: [Live App](https://mattiasmilger.github.io/Web-News-Feed-by-Mattias/) | [GitHub](https://github.com/MattiasMilger/Web-News-Feed-by-Mattias)
- **Väsenväktaren**: [Live App](https://mattiasmilger.github.io/Vasenvaktaren/) | [GitHub](https://github.com/MattiasMilger/Vasenvaktaren)
- **AI Portfolio Optimizer**: [GitHub](https://github.com/MattiasMilger/AI-Portfolio-Optimizer)
- **Reine M (Spotify)**: [Spotify Artist Page](http://open.spotify.com/artist/4ZPJozo56gnUzwzCw2lrrM)

---

## Visual Design & Cyberpunk Harmonics

The page features an ambient cyberpunk aesthetic designed specifically for high visual impact on both desktop and mobile screens:

- **Harmonic Sine Datawaves (Top & Bottom)**:
  - Self-sustaining, continuous multi-frequency harmonic wave readouts that ripple across the top (beneath the subtitle) and the bottom (above the footer).
  - Uses CSS and SVG with organic mathematical sine frequencies that fade smoothly at the left and right edges.
  - Zero cursor or touch tracking: completely self-running at 60fps.
  - Automatically respects `prefers-reduced-motion` for accessibility.
- **Clean Seamless Container Layout**:
  - The main container sits flush and clean without outer glowing borders that would collide with mobile browser scrollbars.
  - In dark mode, cards and links feature subtle neon bloom using the accent colour token (`#2ecc71`).
- **Dynamic Theming**:
  - Fully supports both Dark Mode (default, cyber emerald `#2ecc71`) and Light Mode (cyber blue `#3498db`), dynamically syncing all CSS variables.

---

## Drag-and-Drop Interaction

- **Targeting an Item (Card)**:
  - When clicking and dragging a card, **only that item receives the dashed outline**. The whole category does not get outlined.
  - You can drag cards within a category to reorder them horizontally and vertically, or drag vertically across categories to move the category order.
- **Targeting a Category**:
  - When clicking and dragging a category header directly, the **whole category receives the green dashed outline** (`outline: 2px dashed var(--accent-color)`), and dragging vertically reorders the entire category.
- **Auto-Scrolling & Touch Support**:
  - Dragging near the top or bottom edges of the screen automatically scrolls the page smoothly on touch devices and desktop.
  - Section and card arrangements are saved to `localStorage` and persist between visits.
  - Click **Reset order** in the footer to restore the default layout at any time.

---

## Modular & Removable Effects

All visual effects are encapsulated in clearly marked blocks in `index.html`:

1. **CSS Styles**:
   Look for the `/* ===================================================================== CYBERPUNK EFFECT ... */` block in the `<style>` tag.
2. **HTML Elements**:
   The top and bottom wave containers are marked with `<div class="cyber-datawave-wrap top-wave">` and `<div class="cyber-datawave-wrap bottom-wave">`.
3. **JavaScript Engine**:
   The self-running wave loop is enclosed in `function initDataWaves()`.

To remove the waves or return to a minimal look, simply delete those three labeled blocks.
