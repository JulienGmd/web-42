# Hypertube — Todo

## Mandatory

### Setup
- [ ] Responsive layout: header, main section, footer; mobile-friendly
- [ ] Form validation on all forms; security (no plain-text passwords, no SQL injection, no unwanted uploads, no JS injection)
- [ ] Store credentials in `.env` (gitignored)

### User Interface
- [ ] Registration: email, username, last name, first name, password
- [ ] Omniauth login: 42 strategy + at least 1 other strategy
- [ ] Login with username and password + password reset by email
- [ ] Logout from any page with one click
- [ ] Language selection (defaults to English)
- [ ] Edit email address, profile picture, and other profile info
- [ ] View any other user's profile (profile picture + info; email stays private)

### Library (authenticated users only)
- [ ] Search field querying at least 2 external legal/royalty-free sources
- [ ] Display search results as thumbnails sorted by name
- [ ] Default view: most popular videos from external sources (sorted by chosen criteria)
- [ ] Each thumbnail shows: name, production year (if available), IMDb/OMDb/TMDb rating (if available), cover image
- [ ] Differentiate watched vs. unwatched videos in thumbnails
- [ ] Infinite scroll pagination (next page loaded asynchronously on scroll, no pagination link)
- [ ] List sortable and filterable by name, genre, rating, production year, etc.

### Video page (authenticated users only)
- [ ] Video detail page: player, summary, casting (producer, director, main cast), year, length, IMDb rating, cover image
- [ ] Comment section (users can leave comments; prior comments shown)
- [ ] If not already downloaded, launch the torrent download server-side and start streaming as soon as enough data is buffered (non-blocking, background)
- [ ] Save fully downloaded movies on the server; delete if unwatched for one month
- [ ] Download and display English subtitles if available
- [ ] Download and offer user-language subtitles if the video language differs from user preference and subtitles are available
- [ ] Convert non-browser-readable formats on the fly (minimum: MKV support)

### RESTful API (OAuth2 authentication)
- [ ] `POST /oauth/token` — accepts client + secret, returns auth token
- [ ] `GET /users` — returns list of users (id, username)
- [ ] `GET /users/:id` — returns username, email, profile picture URL (authenticated)
- [ ] `PATCH /users/:id` — update username, email, password, profile picture URL (authenticated)
- [ ] `GET /movies` — returns frontpage top movies (id, name); accessible to any user
- [ ] `GET /movies/:id` — returns name, id, IMDb mark, year, length, available subtitles, comment count
- [ ] `GET /comments` — returns latest comments (author username, date, content, id) (authenticated)
- [ ] `GET /comments/:id` — returns comment, author username, id, date (authenticated)
- [ ] `PATCH /comments/:id` — update comment (authenticated)
- [ ] `DELETE /comments/:id` — delete comment (authenticated)
- [ ] `POST /comments` or `POST /movies/:movie_id/comments` — post a comment (authenticated)
- [ ] Return appropriate HTTP codes for unauthorized/invalid API calls

## Bonus

- [ ] Additional Omniauth strategies
- [ ] Manage multiple video resolutions
- [ ] Stream video via the MediaStream API
- [ ] Add API routes to add/delete movies, etc.
