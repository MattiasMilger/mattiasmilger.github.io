<div align="center">

# Mattias Milger - Portfolio

[![Visit the site](https://img.shields.io/badge/Visit_the_site-mattiasmilger.github.io-2ecc71?style=for-the-badge)](https://mattiasmilger.github.io/)

My projects, all in one place.[cite: 2]

</div>

---

A landing page that links to all of my projects, built with vanilla HTML, CSS, and JavaScript. Runs entirely client-side - no server or backend required. Designed for GitHub Pages.[cite: 2]

**Run locally:** open `index.html` in a modern browser. No build tools or dependencies required.[cite: 2]

### Quick Links (Live Sites & Repositories)
- **Password Generator**: [Live App](https://mattiasmilger.github.io/Web-Password-Generator-by-Mattias/) | [GitHub](https://github.com/MattiasMilger/Web-Password-Generator-by-Mattias)
- **Image Editor**: [Live App](https://mattiasmilger.github.io/Web-Image-Editor-by-Mattias/) | [GitHub](https://github.com/MattiasMilger/Web-Image-Editor-by-Mattias)
- **Local Upload Server**: [GitHub](https://github.com/MattiasMilger/Local-Upload-Server)
- **Flashcards**: [Live App](https://mattiasmilger.github.io/Web-Flashcards-by-Mattias/) | [GitHub](https://github.com/MattiasMilger/Web-Flashcards-by-Mattias)
- **News Feed**: [Live App](https://mattiasmilger.github.io/Web-News-Feed-by-Mattias/) | [GitHub](https://github.com/MattiasMilger/Web-News-Feed-by-Mattias)
- **Väsenväktaren**: [Live App](https://mattiasmilger.github.io/Vasenvaktaren/) | [GitHub](https://github.com/MattiasMilger/Vasenvaktaren)
- **AI Portfolio Optimizer**: [GitHub](https://github.com/MattiasMilger/AI-Portfolio-Optimizer)

<details>
<summary><b>Features</b></summary>

- **Categorized Projects** - Projects are grouped by what they are for (IT, Learning, Games, AI).[cite: 2]
- **Live or Downloadable** - Hosted projects link straight to their `github.io` page, while projects that are not hosted link to GitHub. Live cards have an accent-coloured edge, downloadable cards a grey one.[cite: 2]
- **Availability Filter** - Show all projects, only live ones, or only downloadable ones.[cite: 2]
- **Drag to Reorder** - Drag any section (anywhere except its buttons) to move it. On touch screens, press and hold briefly, then drag. The order is remembered, and a small Reset order button at the bottom restores the default.[cite: 2]
- **Info Window** - An Info button opens a Help & Info window explaining the page, in the same style as my other apps.[cite: 2]
- **Easy to Update** - Every project is one entry in a single list at the top of the script.[cite: 2]
- **Dark / Light Theme** - Toggle between dark and light modes (dark by default). Your choice is remembered.[cite: 2]
- **Responsive Design** - Works on desktop and mobile devices.[cite: 2]

</details>

<details>
<summary><b>Project Structure</b></summary>
mattiasmilger.github.io/
├── index.html      # Page layout, styling (CSS variables), project list, and page logic
└── README.md       # This file
| Part of `index.html` | Purpose |
|---|---|
| `<style>` | Theming (CSS variables), layout, cards, filter buttons, Info window, responsive design[cite: 2] |
| Info window markup | The Help & Info content, shown by the Info button[cite: 2] |
| `PROJECTS` list | The data: one entry per project (category, name, description, app link, repo link)[cite: 2] |
| Script (below the list) | Builds the cards from the list, applies filters, handles dragging and saved order, the Info window, and the theme toggle[cite: 2] |

</details>

<details>
<summary><b>Adding a Project</b></summary>

1. Open `index.html` and find the `PROJECTS` list near the top of the script.[cite: 2]
2. Copy an existing entry and change its values.[cite: 2]
3. Commit and push. GitHub Pages updates within a minute or two.[cite: 2]

| Field | What it does |
|---|---|
| `category` | Section heading. Projects with the same text are grouped together, in the order they first appear. This is the default order; visitors can drag sections to their own order[cite: 2] |
| `name` | Card title[cite: 2] |
| `description` | One or two short sentences[cite: 2] |
| `app` | Link to the hosted `github.io` page, or `null` if the project is not hosted. This also sets the status: a link makes it a **Live** card, `null` makes it a **Downloadable** card[cite: 2] |
| `repo` | Link to GitHub |

If you add a new category, it appears after the sections a visitor has already arranged until they move it.[cite: 2]

</details>

<details>
<summary><b>Hosting on GitHub Pages</b></summary>

This is a GitHub *user site*, so the repository must be named exactly `mattiasmilger.github.io`. It is then served at `https://mattiasmilger.github.io/` with no extra path.[cite: 2]

1. Create a public repository named `mattiasmilger.github.io`.[cite: 2]
2. Add `index.html` and this `README.md` to the root of the `main` branch.[cite: 2]
3. Open **Settings → Pages** and set the source to **Deploy from a branch**, branch `main`, folder `/ (root)`.[cite: 2]

</details>

<details>
<summary><b>Technical Notes</b></summary>

- **No external dependencies** - pure vanilla HTML, CSS, and JavaScript.[cite: 2]
- **Client-side only** - No data is transmitted to any server.[cite: 2]
- **localStorage** - Only two things are stored in the browser: the theme choice (`portfolio_theme`) and the section order (`portfolio_category_order`).[cite: 2]
- **Dragging** - Uses pointer events rather than the browser's built-in drag and drop, so it also works on touch screens.[cite: 2]
- **Status is derived** - A project is "Live" when it has an `app` link, so the badge, card colour, buttons, and filter can never disagree.[cite: 2]
- **Browser support** - Works in all modern browsers (Chrome, Firefox, Edge, Safari). Requires JavaScript enabled.[cite: 2]

</details>

## Credits

**Developer**: Mattias Milger[cite: 2]  
**Email**: mattias.r.milger@gmail.com[cite: 2]  
**GitHub**: [MattiasMilger](https://github.com/MattiasMilger)[cite: 2]