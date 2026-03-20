# PaperMap

PaperMap is a scalable interactive paper library.
The project is now structured so you can keep adding new paper explainers while preserving one consistent homepage style and deployment workflow.

## Repository

- GitHub: https://github.com/AdilShamim8/PaperMap

## Current Scope

- Homepage catalog: `index.html`
- Live paper page: `Attention_Is_All_You_Need.html`
- Project guide: `README.md`

## Design Goal

PaperMap is designed for long-term growth:

- One homepage that lists all papers.
- One standalone HTML page per paper.
- Consistent card-style listing for discoverability.
- Static-first architecture with zero build step.

## Project Structure

```text
PaperMap/
├─ index.html
├─ Attention_Is_All_You_Need.html
├─ favicon.svg
└─ README.md
```

## How To Add A New Paper

1. Create a new HTML page for the paper at repository root.
2. Keep naming clear and predictable (example: `BERT_2018.html`).
3. In `index.html`, add one new card inside the Paper Library section.
4. For each card, include:
	- status tag (`Live` or `Planned`)
	- paper title
	- short summary
	- page link
5. If the new page has its own metadata (title, description, social tags), update those tags in the page head.

## Local Development

### Option 1: Open directly

Open `index.html` in your browser.

### Option 2: Use a local static server

Using Python:

```bash
python -m http.server 8080
```

Then open `http://localhost:8080`

Using Node:

```bash
npx serve .
```

## Deployment

### GitHub Pages

1. Push changes to `main`.
2. In GitHub, open repository settings.
3. Go to Pages.
4. Source: Deploy from a branch.
5. Branch: `main`, folder: `/(root)`.

Live URL:

```text
https://adilshamim8.github.io/PaperMap/
```

### Other Static Hosts

This project also works on Netlify, Vercel static hosting, Azure Static Web Apps, or any static server.

## Maintenance Checklist

Before release:

- Confirm all paper links on homepage cards open correctly.
- Check mobile layout for homepage and each paper page.
- Validate social/contact links and icon visibility.
- Verify favicon renders in browser tab.
- Run a quick accessibility pass (focus states and contrast).

## Attribution

Current live paper is based on:

**Attention Is All You Need**
Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N. Gomez, Lukasz Kaiser, Illia Polosukhin (NeurIPS 2017).

Add your preferred license file if you plan to distribute this project publicly.
