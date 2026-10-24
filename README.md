# Agency Age

A responsive, single-page landing site for the fictional digital agency **Agency Age**, built with Angular, TypeScript, HTML and CSS.

The page recreates the supplied reference design: a slim white header, a two-column hero with a custom flat-vector illustration, four feature cards, and a large gradient footer. Everything is static and frontend-only.

## Tech stack

- Angular 21 (standalone components, no Router)
- TypeScript
- Plain CSS (component styles + global reset)
- No database, forms, authentication or third-party UI libraries

## Getting started

Requirements: Node.js 20.19+, 22.12+ or 24+ and npm.

```bash
npm install
npm start
```

`npm start` is an alias for `ng serve`. Open `http://localhost:4200/` in a browser.

You can also run the Angular CLI directly:

```bash
npx ng serve
```

### Production build

```bash
npm run build
```

The optimized output is written to `dist/agency-age/browser/`.

### Unit tests

```bash
npm test -- --watch=false
```

## Project structure

```text
public/
  favicon.svg
  fonts/plus-jakarta-sans.woff2
  images/hero-illustration.svg
src/
  app/
    app.ts          # Landing-page standalone component
    app.html        # Semantic page template
    app.css         # Page-specific styles and responsive rules
    app.spec.ts
  index.html
  main.ts
  styles.css        # Global reset, typeface and base defaults
```

Angular 21 serves files from `public/` at the application root, so the illustration is referenced as `images/hero-illustration.svg`.

