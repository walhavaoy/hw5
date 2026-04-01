# Tech Stack

## Runtime
- **Node.js**: >= 18.x
- **TypeScript**: ~5.x (strict mode)

## Framework
- **Express**: ~4.x (HTTP server and routing)

## Dependencies

### Production
| Package   | Version | Purpose              |
|-----------|---------|----------------------|
| express   | ^4.18   | HTTP server/routing  |
| pino      | ^8.x    | Structured logging   |

### Development
| Package      | Version | Purpose               |
|--------------|---------|----------------------|
| typescript   | ^5.x    | TypeScript compiler   |
| @types/express | ^4.x  | Express type defs     |
| @types/node  | ^20.x   | Node.js type defs     |

## Build Toolchain
- **Compiler**: `tsc` (TypeScript compiler)
- **Output**: `dist/` directory
- **Target**: ES2022 / Node16 module resolution

## Client Side
- Vanilla JavaScript (no framework, no bundler)
- Inline in HTML served by Express
