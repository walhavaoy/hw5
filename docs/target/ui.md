# UI Specification

## Page Inventory

Single page served at `GET /`.

## Component Hierarchy

```
Page (body)
  +-- Heading ("Hello World")          [data-testid="heading"]
  +-- Server Time Display              [data-testid="server-time"]
  +-- Greeting Button                  [data-testid="greeting-button"]
  +-- Greeting Display Area            [data-testid="greeting-display"]
```

## Interaction Flows

### Greeting Fetch
1. User clicks the greeting button
2. Client JS sends `fetch('/api/greeting')`
3. Response JSON is parsed
4. `greeting` value is displayed in the greeting display area

## Styling

- **Theme**: Dark background with warm accent colors
- **Colors**: CSS custom properties for theming
- **Layout**: Centered content, fluid widths
- **Responsive**: Viewport meta tag, fluid CSS (rem units, max-width)
- **Font**: System font stack

## data-testid Attributes

| Element            | data-testid          |
|--------------------|----------------------|
| Main heading       | `heading`            |
| Server time        | `server-time`        |
| Greeting button    | `greeting-button`    |
| Greeting display   | `greeting-display`   |
