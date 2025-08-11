## Usage

### Run locally

- Open `index.html` in your browser, or
- Serve the directory with a static server:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

### Editing styles

- Add your CSS rules to `style.css`.
- Link additional stylesheets in `index.html` if needed.

### Adding JavaScript

- Create a `script.js` and include it in `index.html` with:

```html
<script src="script.js" defer></script>
```

- Prefer organizing code into small, well-named functions and documenting them with JSDoc.

### Deployment

- Host the files on any static host (GitHub Pages, Netlify, Vercel, S3, etc.).
- Ensure the entry point is `index.html` at the project root.