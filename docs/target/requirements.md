# Requirements

## Functional Requirements

### REQ-01-01: Hello World Page
- **Priority**: must
- **Type**: functional
- `GET /` serves an HTML page with a "Hello World" heading

### REQ-01-02: Random Greeting API
- **Priority**: must
- **Type**: functional
- `GET /api/greeting` returns a random greeting as JSON (`{ greeting: string }`)

### REQ-01-03: Greeting Button
- **Priority**: must
- **Type**: functional
- A button on the page calls `GET /api/greeting` and displays the result

### REQ-01-04: Server Time Display
- **Priority**: must
- **Type**: functional
- The page displays the current server time at page load

## Non-Functional Requirements

### REQ-02-01: Dark Theme
- **Priority**: must
- **Type**: non-functional
- Dark theme with warm color palette

### REQ-02-02: Mobile Responsive
- **Priority**: must
- **Type**: non-functional
- Mobile responsive layout using viewport meta tag and fluid CSS

### REQ-02-03: Test IDs
- **Priority**: must
- **Type**: non-functional
- All interactive elements have `data-testid` attributes

### REQ-02-04: Single File Server
- **Priority**: must
- **Type**: non-functional
- Single file server implementation in `src/index.ts`

### REQ-02-05: Port 3000
- **Priority**: must
- **Type**: non-functional
- Server listens on port 3000

### REQ-02-06: No Database
- **Priority**: must
- **Type**: non-functional
- No database dependency; fully self-contained

### REQ-02-07: Vanilla JS Client
- **Priority**: must
- **Type**: non-functional
- Vanilla JS only on the client side (no frontend framework)
