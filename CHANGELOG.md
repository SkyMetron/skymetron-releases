# Changelog

## v0.2.8-beta (2026-07-13)

### Highlights

- New login-first flow with GitHub Device Flow
- Owner-only access via Joao-Aschenbrenner (ID 71678259)
- Token protected by Windows DPAPI
- Session restoration after restart
- Doctor/Docker/workspace blocked until owner authentication
- Device Flow with user code display and copy
- All tests passing: 265 backend, 13 auth, 11 Playwright/Electron
- Gitleaks: 0 leaks
- npm audit: 3 known advisories (electron, vite, esbuild)

### Not Included

- Docker bootstrap
- Workspaces
- Graphify/OpenCode/OPA/Temporal
- Private repositories
