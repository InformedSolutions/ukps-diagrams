# UK PharmaScan LikeC4 Diagrams

This repository contains a LikeC4 model for **UK PharmaScan (UKPS)** based on the supplied C4 context and container summary.

## Views

- `UK PharmaScan System Context`
- `UK PharmaScan Container View`
- `UK PharmaScan Backend API Components`

## Files

- `src/model.c4`: UKPS model
- `src/model.views.c4`: context, container, and backend component views
- `src/_spec.c4`: small project-specific element conventions
- `assets/logos/`: local SVG logos used by the diagram elements

## Usage

Install dependencies:

```bash
npm install
```

Start the local preview server:

```bash
npm run dev
```

Validate the model:

```bash
npm run validate
```

Build a static site:

```bash
npm run build
```

Export PNGs:

```bash
npm run export:png
```

## Notes

- The model follows the current LikeC4 template structure: `likec4.config.ts`, `src/model.c4`, `src/model.views.c4`.
- On this machine, `node -v` is `v20.19.0`. The current `likec4@1.53.0` package reports an engine warning for Node 22.x, but the CLI is still invokable here with `npx`. If `npm install` fails in your environment, upgrade Node first.
- Vendor and platform logos were pulled from public upstream assets. The UK PharmaScan mark in `assets/logos/ukps.svg` is a simplified local recreation based on the official leaflet cover because the site did not expose a directly downloadable logo asset cleanly.
