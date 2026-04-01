# Component Taxonomy and Priority Matrix

## Components

| ID | Component | Priority | Phase | Status |
|----|-----------|----------|-------|--------|
| C-01 | Project scaffolding (package.json, tsconfig.json) | must | Phase 1 | pending |
| C-02 | Express server skeleton (src/index.ts) | must | Phase 1 | pending |
| C-03 | GET / HTML route with heading | must | Phase 2 | pending |
| C-04 | Server time display | must | Phase 2 | pending |
| C-05 | GET /api/greeting endpoint | must | Phase 2 | pending |
| C-06 | Greeting button + client JS | must | Phase 2 | pending |
| C-07 | data-testid attributes | must | Phase 2 | pending |
| C-08 | Dark warm-palette theme | must | Phase 3 | pending |
| C-09 | Mobile responsive layout | must | Phase 3 | pending |

## Dependency Order

```
C-01 -> C-02 -> C-03 -> C-04
                    \-> C-05 -> C-06
                    \-> C-07
C-03 -> C-08 -> C-09
```

## Phase Summary

- **Phase 1**: Project Setup (C-01, C-02)
- **Phase 2**: Core Routes & HTML (C-03, C-04, C-05, C-06, C-07)
- **Phase 3**: Styling & Polish (C-08, C-09)
- **Phase 4**: Verification (build + test)
