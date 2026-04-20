# Camagru — Todo

## Mandatory

### Setup
- [ ] Containerize the app (docker-compose or equivalent, deployable with one command)
- [ ] Responsive layout: header, main section, footer; mobile-friendly
- [ ] Form validation on all forms
- [ ] Security: hashed passwords, no HTML/JS injection, no unwanted uploads, no SQL injection, no CSRF

### User features
- [ ] Registration: email, username, password (with complexity requirement)
- [ ] Account confirmation via unique link sent by email
- [ ] Login with username and password
- [ ] Password reset by email
- [ ] Logout from any page with one click
- [ ] Edit username, email, and password when logged in

### Gallery
- [ ] Public gallery displaying all users' edited images ordered by creation date
- [ ] Like and comment on images (connected users only)
- [ ] Email notification to image author on new comment (default on, deactivatable in preferences)
- [ ] Paginate gallery (minimum 5 images per page)

### Editing (authenticated users only)
- [ ] Main section: webcam preview, list of selectable superposable images, capture button
- [ ] Capture button inactive until a superposable image is selected
- [ ] Side section: thumbnails of the user's previously taken pictures
- [ ] Image composition (superposing webcam + selected image) done server-side
- [ ] Allow image upload as alternative to webcam capture
- [ ] Allow users to delete only their own edited images

## Bonus

- [ ] AJAXify exchanges with the server
- [ ] Live preview of the superposed result directly on the webcam feed
- [ ] Infinite scroll pagination for the gallery
- [ ] Share images on social networks
- [ ] Render an animated GIF
