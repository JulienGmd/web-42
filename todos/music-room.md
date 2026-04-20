# Music Room — Todo

## Mandatory

### User
- [ ] Account creation: email/password or social network (Facebook or Google)
- [ ] Link Facebook or Google account to an existing account
- [ ] Profile: public info, friends-only info, private info, music preferences (all editable)
- [ ] Email validation on registration (email/password accounts)
- [ ] Password reset by email (email/password accounts)

### Services (implement at least 2 of the 3 below)

#### Music Track Vote
- [ ] Users can suggest or vote for the next track in the current playlist
- [ ] Tracks with more votes rise in the playlist order
- [ ] Public/private event visibility (default: public; private = invited users only)
- [ ] License management: open voting (default), invited-only voting, location+time-based voting
- [ ] Handle concurrent vote conflicts (e.g., simultaneous votes on same/different tracks)

#### Music Control Delegation
- [ ] User can delegate music control to different friends
- [ ] License management per device attached to the user's account

#### Music Playlist Editor
- [ ] Real-time multi-user collaborative playlist editing
- [ ] Public/private playlist visibility (default: public; private = invited users only)
- [ ] License management: open editing (default), invited-users-only editing
- [ ] Handle concurrent edit conflicts (e.g., simultaneous moves of tracks)

### Server
- [ ] All service data stored on the backend (backend is the single source of truth)

### API
- [ ] RESTful API (be able to justify the choice and explain its characteristics)
- [ ] JSON as exchange format (be able to justify the choice)
- [ ] API documentation covering methods, inputs, and outputs (e.g., Swagger)

### Mobile application
- [ ] Mobile app for Android or iOS covering all project actions
- [ ] App acts as a remote control to the backend; backend address is configurable
- [ ] Social network authentication (Facebook or Google) in the mobile app

### Securing
- [ ] Users can only access their own data (access control)
- [ ] Protection against brute-force attacks on the API
- [ ] Protection against session theft
- [ ] Identify and document other security hazards and their mitigations
- [ ] Log every mobile action on the backend (platform, device model, app version)

### Ramp-up
- [ ] Load test the API and backend (using AB, Gatling, Siege, Tsung, JMeter, or similar)
- [ ] Document server characteristics (CPU, RAM, cloud/on-premise) and justify the measured user capacity

### Agility & CI
- [ ] Unit tests for each layer of the application

## Bonus

- [ ] Multi-platform support: make the service available as a responsive web app
- [ ] IBeacon/IoT: automatically notify nearby users about public events
- [ ] Free vs. paid subscription tiers (some features locked to paid plan)
- [ ] Offline mode with sync (handle conflicts and obsolete data on re-connect)
