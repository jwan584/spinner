# AGENTS.md

## Project overview

**Pentagon Physics Simulator** — a client-side web app that simulates colorful balls bouncing inside a slowly rotating pentagon. It uses [Matter.js](https://brm.io/matter-js/) (loaded from CDN) with no build step, backend, or package manager.

The `main` branch currently contains only a placeholder `README.md`. The runnable application lives on feature branches:

| Branch | Notes |
|--------|-------|
| `cursor/unitary-pentagon-9573` | Recommended — balls render and physics work end-to-end |
| `cursor/pentagon-physics-simulator-905f` | Earlier variant; pentagon and controls work, but ball rendering may not appear in all browsers |

## Cursor Cloud specific instructions

### Checkout before running

```bash
git checkout cursor/unitary-pentagon-9573
```

### Start the dev server

From the repo root (see [README on the feature branch](README.md)):

```bash
python3 -m http.server 8080
```

Then open http://localhost:8080 in a browser. A hard refresh (`Ctrl+Shift+R`) may be needed after switching branches while the server is already running.

### Services

| Service | Required | How to start |
|---------|----------|--------------|
| Static HTTP server | Recommended | `python3 -m http.server 8080` |
| Web browser | Required | Visit http://localhost:8080 |
| CDN (cdnjs.cloudflare.com) | Required | Outbound HTTPS; loads Matter.js at runtime |

No Docker, database, or Node.js tooling is needed.

### Lint / test / build

There are no automated linters, test suites, or build commands in this repository. Verification is manual: confirm the page loads, balls are visible inside the pentagon, and the Rotation/Gravity sliders plus Add Ball / Reset buttons respond.

### Environment variables

None required.
