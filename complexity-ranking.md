# Projects Ranked by Implementation Complexity

From easiest to hardest.

---

## 1. Darkly — ~1–2 weeks - 6300 XP

Research/CTF project: no app to build. Find and document 14 security breaches on a pre-built website, explain each exploit, and be ready to patch them. The bulk of work is investigation, not development.

**Key challenges:** breadth of vulnerability types to master (SQLi, XSS, CSRF, etc.), manual exploitation (no sqlmap).

---

## 2. Camagru — ~3–4 weeks - 4200 XP

Classic fullstack web app: auth (registration, email confirmation, password reset), image editing (webcam capture + server-side image superposition), public gallery with likes/comments and email notifications.

**Key challenges:** server-side image composition, webcam integration, email sending.

---

## 3. Red Tetris — ~4–6 weeks - 15750 XP

Multiplayer Tetris with strict architectural constraints: functional client (no `this`), OOP server with prototypes, Redux state management, socket.io real-time sync, and ≥70% unit test coverage.

**Key challenges:** Tetris game logic (rotation, collision, penalty lines), synchronized piece sequences across players, meeting the 70% coverage threshold.

---

## 4. Matcha — ~6–8 weeks - 9450 XP

Dating app with complex matching logic, real-time chat and notifications (≤10s delay), geolocation, like/block/report system, and manual SQL queries (no ORM). Requires seeding 500 distinct profiles for evaluation.

**Key challenges:** matching algorithm (proximity + tags + fame rating), real-time WebSocket infrastructure for both chat and notifications, no ORM constraint, GPS handling.

---

## 5. Hypertube — ~8–10 weeks - 15750 XP

Video streaming platform: torrent-based downloading with in-browser streaming (starts as soon as enough data is buffered), on-the-fly format conversion (MKV → browser-readable), multi-source search (2+ external APIs), subtitles, OAuth2 (42 + 1 other), and a full REST API.

**Key challenges:** torrent streaming pipeline, on-the-fly transcoding, integrating multiple external video/metadata sources, OAuth2 + REST API layer.

---

## 6. Music Room — ~10–14 weeks - 25200 XP

The most complex project: requires a **mobile app** (Android or iOS) in addition to a backend + REST API. Must implement 2 of 3 complex real-time services (track voting with conflict resolution, music control delegation, collaborative playlist editing). Also requires load testing, CI with unit tests, and full API documentation.

**Key challenges:** mobile development, concurrent conflict resolution for real-time collaborative features, load testing and capacity planning, social auth (Facebook/Google) on both web and mobile.
