# Matcha — Todo

## Mandatory

### Setup
- [ ] Responsive layout: header, main section, footer; mobile-friendly
- [ ] Form and upload validation; security (hashed passwords, no SQL injection, no JS/HTML injection, no unwanted uploads)
- [ ] Manual SQL queries (no ORM); relational or graph-oriented database
- [ ] Database seeded with at least 500 distinct profiles for evaluation
- [ ] Store credentials in `.env` (gitignored)

### Registration & Sign-in
- [ ] Registration: email, username, last name, first name, password (no common dictionary words)
- [ ] Email verification via unique link after registration
- [ ] Login with username and password
- [ ] Password reset by email
- [ ] Logout from any page with one click

### User profile
- [ ] Set/edit: gender, sexual preferences, biography, interest tags (reusable, e.g. #vegan), up to 5 pictures (1 as profile picture)
- [ ] Edit: last name, first name, email address
- [ ] View list of users who visited their profile
- [ ] View list of users who liked them
- [ ] Public fame rating (definition at developer's discretion, must be consistent)
- [ ] GPS location with explicit user consent; manual location input (city/neighborhood) if GPS refused
- [ ] Allow user to modify their location from their profile at any time

### Browsing
- [ ] Suggest profiles matching user's sexual preferences (handle hetero, homo, bi; default bisexual if unspecified)
- [ ] Match based on: geographic proximity, number of shared tags, fame rating; prioritize same area
- [ ] Suggested list sortable by age, location, fame rating, common tags
- [ ] Suggested list filterable by age, location, fame rating, common tags

### Research
- [ ] Advanced search by: age range, fame rating range, location, interest tags (one or more)
- [ ] Search results sortable and filterable by age, location, fame rating, interest tags

### Profile view
- [ ] Display all profile info except email and password
- [ ] Record profile visit in the viewed user's history
- [ ] Like another user's profile picture (requires own profile picture; triggers connection if mutual)
- [ ] Unlike/remove a previously given like (disables chat and future notifications from that user)
- [ ] Check another user's fame rating
- [ ] See whether a user is currently online; if not, show date and time of last connection
- [ ] Report a user as a fake account
- [ ] Block a user (removes from search results, stops notifications, disables chat)
- [ ] Show clearly if the viewed profile has liked you and/or if you are connected; option to unlike/disconnect

### Chat
- [ ] Real-time chat between mutually liked (connected) users
- [ ] New message indicator visible from any page

### Notifications (real-time, max 10s delay)
- [ ] Notification when receiving a like
- [ ] Notification when profile is viewed
- [ ] Notification when receiving a message
- [ ] Notification when a liked user likes back (mutual like)
- [ ] Notification when a connected user unlikes you
- [ ] Unread notification indicator visible from any page

## Bonus

- [ ] OmniAuth strategies for user authentication
- [ ] Personal photo gallery with drag-and-drop upload and basic image editing (crop, rotate, filters)
- [ ] Interactive map of users with precise GPS localization via JavaScript
- [ ] Video or audio chat for connected users
- [ ] Feature to schedule and organize real-life dates or events for matched users
