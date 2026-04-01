# API Contracts

## GET /

Serves the main HTML page.

- **Response**: `text/html`
- **Status**: 200
- **Content**: HTML page containing:
  - "Hello World" heading (`data-testid="heading"`)
  - Server time display (`data-testid="server-time"`)
  - Greeting button (`data-testid="greeting-button"`)
  - Greeting display area (`data-testid="greeting-display"`)

## GET /api/greeting

Returns a random greeting from a hardcoded list.

- **Response**: `application/json`
- **Status**: 200
- **Schema**:
```json
{
  "greeting": "string"
}
```
- **Example Response**:
```json
{
  "greeting": "Welcome, friend!"
}
```
