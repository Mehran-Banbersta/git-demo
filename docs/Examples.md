## Examples

### Add a button that shows an alert

```html
<!-- index.html -->
<body>
  <h1>Git Demo</h1>
  <button id="helloBtn">Say hello</button>
  <script>
    document.getElementById('helloBtn').addEventListener('click', () => {
      alert('Hello from Git Demo!');
    });
  </script>
</body>
```

### Split JavaScript into a separate file

```html
<!-- index.html -->
<script src="script.js" defer></script>
```

```javascript
// script.js
export function greet(name) {
  return `Hello, ${name}!`;
}

document.addEventListener('DOMContentLoaded', () => {
  console.log(greet('world'));
});
```

### Basic responsive layout with CSS

```css
/* style.css */
:root {
  --space: 1rem;
}

body {
  margin: 0;
  padding: var(--space);
  display: grid;
  gap: var(--space);
}

@media (min-width: 768px) {
  body {
    grid-template-columns: 1fr 3fr;
  }
}
```