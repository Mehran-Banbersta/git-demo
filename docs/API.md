## API Reference

As of now, the repository contains only static HTML/CSS and defines no public JavaScript APIs, functions, or classes.

When you introduce JavaScript, document public APIs here. Use the following guidance.

### What counts as a public API?

- Functions, classes, or objects intended to be imported or called from outside their defining module
- Global functions exposed to the page
- Events or custom DOM attributes that other code can rely on

### Documentation template (JSDoc style)

```javascript
/**
 * Short description of what the function does.
 *
 * @param {string} input - Description of the input parameter.
 * @param {number} [timeoutMs=1000] - Optional parameter with default.
 * @returns {Promise<Result>} Description of the resolved value.
 * @throws {Error} Conditions under which the function throws.
 * @example
 * await doThing("hello", 500);
 */
export async function doThing(input, timeoutMs = 1000) { /* ... */ }
```

### Example: component initializer API

```javascript
/** Initialize the banner component on the page. */
export function initBanner(options) { /* ... */ }

// Usage
import { initBanner } from "./banner.js";
initBanner({ theme: "light" });
```

### Versioning and stability

- Use semantic versioning when you begin publishing builds
- Mark experimental APIs with `@experimental`
- Deprecate with `@deprecated` and document migration paths