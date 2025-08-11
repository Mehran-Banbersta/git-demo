## Components and Structure

### Page: `index.html`

High-level structure:

```1:12:/workspace/index.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>
  <h1>Git Demo</h1>
</body>
</html>
```

#### Components

- **Heading (`<h1>`)**: Displays the page title "Git Demo".
- **Head metadata**: Standard meta tags for charset, IE compatibility, and viewport.

### Styles: `style.css`

- The stylesheet exists but is currently empty. Add rules to style the page. Example:

```css
/* style.css */
body {
  font-family: system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, sans-serif;
  margin: 0;
  padding: 2rem;
}

h1 {
  color: #1a73e8;
}
```

### Conventions

- Keep markup semantic (use headings, sections, articles appropriately).
- Keep components small and reusable. If components grow complex, consider introducing a framework or templating system.