# Hello World Express App

## Overview
A minimal Hello World web application using Node.js/Express with TypeScript. Displays a heading, shows server time, and fetches random greetings via a button click. Styled with a dark warm-palette theme.

## Tech Stack
- **Runtime**: Node.js with TypeScript
- **Framework**: Express.js
- **Build**: tsc (TypeScript compiler)
- **Port**: 3000

## Directory Structure
```
/
  src/
    index.ts        # Single-file Express server (all routes + inline HTML)
  package.json
  tsconfig.json
  CLAUDE.md
  docs/
    target/         # Requirements and design specs
    implemented/    # Coverage tracking
```

## Build / Run / Test
```bash
npm install          # Install dependencies
npm run build        # Compile TypeScript (tsc)
npm start            # Run the compiled server (node dist/index.js)
npm run dev          # Run with ts-node for development (if configured)
npm test             # Run tests (if configured)
```

## Code Conventions
- TypeScript strict mode enabled
- Use `pino` for structured logging (never console.log)
- Prefix unused function parameters with underscore (e.g. `_req`, `_res`)
- No `any` types; define interfaces for all data shapes
- Handle errors explicitly; log with `logger.error({ err }, message)`
- Single-file server: all routes and HTML live in `src/index.ts`
- Inline HTML served from Express routes (no template engine)
- Vanilla JS only on the client side (no frontend frameworks)
- All interactive elements must have `data-testid` attributes
- No database; fully self-contained

## Key Design Decisions
- Server time is rendered once at page load (not live-updating)
- Random greetings are served from a hardcoded list in the server
- HTML, CSS, and client JS are all inline in the Express route handler
- Dark theme with warm color palette using CSS custom properties
- Mobile responsive via viewport meta tag and fluid CSS

## Routes
- `GET /` — Serves the HTML page with heading, server time, and greeting button
- `GET /api/greeting` — Returns `{ greeting: string }` with a random greeting
