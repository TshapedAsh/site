# Futuristic Portfolio Website

This is a modern SvelteKit-based portfolio template styled with Tailwind CSS. It includes light and dark modes with glassmorphism effects and subtle animations.

## Pages
- **Home** (`/`)
- **Projects** (`/projects`)
- **About** (`/about`)
- **Blog** (`/blog`)
- **Gallery** (`/gallery`)

## Customizing
1. **Content**
   - Edit the Svelte files in `src/routes` to update page content.
   - Reusable components live in `src/lib`.
2. **Theme**
   - Use the toggle in the top-right corner to switch themes. Edit `src/lib/stores/theme.ts` for defaults.
3. **Assets**
   - Upload PDFs to `static/assets/pdfs`.
   - Upload general images to `static/assets/images`.
   - Gallery images go in `static/assets/gallery`.
   - Logos and favicons go in `static/assets/logos`.
   - Replace the placeholder files with your own.
4. **Favicons**
   - Use a square PNG named `favicon.png` (512×512 recommended) in `static/`.
   - Logos should be placed in `static/assets/logos` following the same naming scheme, e.g. `my-logo.png`.

## Development
Install dependencies and start the dev server:

```bash
npm install
npm run dev -- --open
```

## Deployment
This project uses **adapter-static** for compatibility with Vercel, Netlify or GitHub Pages.

### GitHub Pages
1. Push the repository to GitHub.
2. Enable GitHub Pages in the repository settings (deploy from `gh-pages` branch).
3. The included GitHub Actions workflow builds and deploys automatically.

### Vercel / Netlify
- Import the repository and follow the provider’s instructions.
- Ensure the build command is `npm run build` and the output directory is `build`.

## License
[MIT](LICENSE)
