# PaperMap

PaperMap is a production-style interactive learning website for the paper **Attention Is All You Need** (Vaswani et al., 2017).
It turns dense research concepts into clear visual modules, with guided sections, dynamic demos, architecture maps, and comprehension quizzes.

## Live Entry Points

- `index.html`: Product landing page for PaperMap.
- `Attention_Is_All_You_Need.html`: Full interactive explainer (core application).

## Repository

- GitHub: https://github.com/AdilShamim8/PaperMap

## Highlights

- End-to-end narrative for Transformer fundamentals.
- Interactive modules for tokenization, embeddings, attention, architecture, and optimization.
- Accessible baseline with semantic structure, skip link, keyboard-friendly controls, and reduced-motion support.
- Static-site architecture with zero build step and simple deployment.

## Project Structure

```text
PaperMap/
├─ index.html
├─ Attention_Is_All_You_Need.html
└─ README.md
```

## Local Development

This project can run directly as static files.

### Option 1: Open directly

Open `index.html` in a browser.

### Option 2: Run with a local server (recommended)

Using Python:

```bash
python -m http.server 8080
```

Then open: `http://localhost:8080`

Using Node (if installed):

```bash
npx serve .
```

## Deployment

### GitHub Pages

1. Push this folder to a GitHub repository.
2. Open **Settings** -> **Pages**.
3. Set **Source** to **Deploy from a branch**.
4. Select branch `main` and folder `/(root)`.
5. Save and wait for deployment.

Site URL format:

```text
https://adilshamim8.github.io/PaperMap/
```

### Other Static Hosts

You can deploy this project as-is to Netlify, Vercel (static), Azure Static Web Apps, or any Nginx/Apache static host.

## Production Notes

- Keep file names stable to avoid broken links.
- Prefer self-hosting fonts if you need strict offline or CSP policies.
- For SEO previews, add a real Open Graph image URL for your domain.
- Run Lighthouse checks before each release.

## Content and Branding Customization

- Update branding text in `index.html` and the navigation area of `Attention_Is_All_You_Need.html`.
- Update metadata tags (`title`, `description`, and Open Graph fields) for your domain.
- Tune section copy and examples for your audience (students, engineers, interview prep, etc.).

## Quality Checklist

Before publishing, verify:

- All section links in the top navigation scroll correctly.
- Mobile layout is usable at widths between 360px and 430px.
- Interactive demos render and update without console errors.
- Quiz interactions and chart drawing functions execute correctly.
- Keyboard tab order remains clear and predictable.

## License and Attribution

This project is an educational visualization of ideas from:

**Attention Is All You Need**
Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N. Gomez, Lukasz Kaiser, Illia Polosukhin (NeurIPS 2017).

Add your preferred license in this repository if you plan to distribute or reuse this work publicly.
