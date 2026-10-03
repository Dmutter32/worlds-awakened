# Worlds Awakened

A cooperative browser-game prototype for 2–4 players. Explore a riverside frontier landing, share observations and work together to restore unfamiliar machinery.

## Build and run

Requires Node.js 24.

```sh
npm ci --include=dev
npm run build
npm start
```

The server serves the browser client and authoritative multiplayer together. Production hosting must support HTTPS and WebSockets. Players create or join anonymous rooms using a room code; no game account is required. Temporary rooms live in server memory and end if the server process restarts.

For Render, use Free compute, the build/start commands above and `/health` as the health-check path. No database or persistent disk is required. Do not enable paid resources.

This is a development prototype; final visual/audio polish and public-device verification are ongoing. Third-party notices are in `THIRD_PARTY_NOTICES.md`.
