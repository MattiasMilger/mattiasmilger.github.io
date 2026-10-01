# Mattias Milger - Portfolio

A landing page that links to all of my projects: web apps, a game and desktop tools. Built with vanilla HTML, CSS, and JavaScript. Runs entirely client-side - no server or backend required. Designed for GitHub Pages.

## Try It Out

The live version is available at: **https://mattiasmilger.github.io/**

### Run Locally

Open `index.html` in a modern browser. No build tools or dependencies required.

## Features

- **Categorized Projects** - Projects are grouped by purpose (IT admin & security, Games, Learning & reading, Finance & AI).
- **Live or Source Only** - Hosted projects link straight to their `github.io` page, while projects that are not hosted link to their GitHub repository.
- **Availability Filter** - Show all projects, only live ones, or only source-only ones.
- **Language Filter** - Filter by programming language. Buttons are generated automatically from the project list.
- **Easy to Update** - Every project is one entry in a single list at the top of the script.
- **Dark / Light Theme** - Toggle between dark and light modes (dark by default). Your choice is remembered.
- **Responsive Design** - Works on desktop and mobile devices.

## Project Structure

```
mattiasmilger.github.io/
├── index.html      # Page layout, styling (CSS variables), project list, and filter logic
└── README.md       # This file
```

### Module Responsibilities

| Part of `index.html` | Purpose |
|---|---|
| `<style>` | Theming (CSS variables), layout, cards, filter buttons, responsive design |
| `PROJECTS` list | The data: one entry per project (category, name, language, description, app link, repo link) |
| Script (below the list) | Builds the cards from the list, creates the language filters, applies filters, handles the theme toggle |

## Adding a Project

1. Open `index.html` and find the `PROJECTS` list near the top of the script.
2. Copy an existing entry and change its values.
3. Commit and push. GitHub Pages updates within a minute or two.

| Field | What it does |
|---|---|
| `category` | Section heading. Projects with the same text are grouped together, in the order they first appear |
| `name` | Card title |
| `language` | Badge text and language filter. A new language gets its own filter button automatically |
| `description` | One or two short sentences |
| `app` | Link to the hosted `github.io` page, or `null` if the project is not hosted. This also sets the status: a link makes it a **Live** card, `null` makes it a **Source only** card |
| `repo` | Link to the GitHub repository |

## Hosting on GitHub Pages

This is a GitHub *user site*, so the repository must be named exactly `mattiasmilger.github.io`. It is then served at `https://mattiasmilger.github.io/` with no extra path.

1. Create a public repository named `mattiasmilger.github.io`.
2. Add `index.html` and this `README.md` to the root of the `main` branch.
3. Open **Settings → Pages** and set the source to **Deploy from a branch**, branch `main`, folder `/ (root)`.

## Technical Notes

- **No external dependencies** - pure vanilla HTML, CSS, and JavaScript.
- **Client-side only** - No data is transmitted to any server.
- **localStorage** - Only the theme choice (`portfolio_theme`) is stored in the browser.
- **Status is derived** - A project is "Live" when it has an `app` link, so the badge, card colour, buttons, and filter can never disagree.

## Browser Support

Works in all modern browsers (Chrome, Firefox, Edge, Safari). Requires JavaScript enabled.

## Credits

**Developer**: Mattias Milger  
**Email**: mattias.r.milger@gmail.com  
**GitHub**: [MattiasMilger](https://github.com/MattiasMilger)
