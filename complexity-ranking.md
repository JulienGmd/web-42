# Projects Ranked by Implementation Complexity

| # | Project    | Duration     | XP    | Shareable         |
| - | ---------- | ------------ | ----- | ----------------- |
| 1 | Darkly     | ~1–2 weeks   | 6300  | —                 |
| 2 | Camagru    | ~3–4 weeks   | 4200  | ⚠️ isolated        |
| 3 | Red Tetris | ~4–6 weeks   | 15750 | ⚠️ isolated        |
| 4 | Matcha     | ~6–8 weeks   | 9450  | ✅ with Hypertube |
| 5 | Hypertube  | ~8–10 weeks  | 15750 | ✅ with Matcha    |
| 6 | Music Room | ~10–14 weeks | 25200 | ✅ backend only   |

## 1. Darkly

No code. Find and document 14 security breaches on a pre-built website, explain each exploit, be ready to patch them.

- **Challenges:** breadth of vulnerability types (SQLi, XSS, CSRF…), manual exploitation only

## 2. Camagru

Auth (register + email confirm + password reset), webcam capture, server-side image superposition, public gallery with likes/comments/email notifications.

- **Challenges:** server-side image composition, webcam integration, email sending
- **Stack:** any language (PHP stdlib equivalents only), vanilla JS + HTML/CSS (CSS frameworks ok), docker-compose
- Most restrictive stack — no sharing with other projects

## 3. Red Tetris

Multiplayer Tetris: functional client, OOP server, Redux state, socket.io sync, ≥70% unit test coverage.

- **Challenges:** game logic (rotation, collision, penalty lines), synchronized piece sequences, coverage threshold
- **Stack:** Node.js (OOP `Player`/`Piece`/`Game` classes), React or Vue SPA + Redux, socket.io, ≥70% stmt/fn/line coverage
- JS-only constraint — no auth system to reuse

## 4. Matcha

Dating app: matching algorithm, real-time chat + notifications (≤10s), geolocation, like/block/report, 500 seed profiles.

- **Challenges:** matching algorithm (proximity + tags + fame rating), WebSocket infra for chat + notifications, raw SQL, GPS
- **Stack:** any language + micro-framework with router only (Express, Flask, Slim…), any UI lib, relational or graph DB (raw SQL), WebSockets, email/password auth + verification

## 5. Hypertube

Video platform: torrent download + in-browser streaming, on-the-fly transcoding (MKV+), 2+ external sources, subtitles, Omniauth, REST API + OAuth2.

- **Challenges:** torrent streaming pipeline, on-the-fly transcoding, multiple external APIs, OAuth2 + REST layer
- **Stack:** any language + any framework, any UI lib + DB, email/password + Omniauth (42 + 1 other), OAuth2-authenticated REST API
- Add OAuth on top of the Matcha auth/user/profile base

## 6. Music Room

Mobile app + backend + REST API. 2 of 3 real-time services: track voting, music control delegation, collaborative playlist editing. Load testing + unit tests + API docs.

- **Challenges:** mobile development, concurrent conflict resolution, load testing + capacity planning, social auth on mobile
- **Stack:** any language/framework, Android or iOS (React Native, Flutter, Swift, Kotlin…), Facebook/Google OAuth, REST + JSON + Swagger, WebSockets, unit tests + load testing (AB, Gatling, JMeter…)
- Backend patterns overlap with Matcha/Hypertube — no frontend reuse due to mobile
