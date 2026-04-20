# Red Tetris — Todo

## Mandatory

### Game mechanics
- [ ] Standard Tetris on a 10×20 grid with the 7 original Tetrimino shapes and rotation rules
- [ ] All players in the same game receive the same piece sequence
- [ ] Clearing lines sends n−1 indestructible penalty lines to the bottom of each opponent's field
- [ ] Each player sees opponents' names and a real-time spectrum view (column heights)
- [ ] No scoring system; last remaining player wins
- [ ] Support both solo (1 player) and multiplayer modes

### Piece movement
- [ ] Left/Right arrows: move piece horizontally
- [ ] Up arrow: rotate piece
- [ ] Down arrow: soft drop
- [ ] Spacebar: hard drop
- [ ] Piece becomes immobile on the next frame after touching the pile (allows last-moment adjustments)

### Architecture & tech constraints
- [ ] Full Stack JavaScript (TypeScript allowed)
- [ ] Client-side: no `this` keyword (functional approach); pure functions for board/piece logic
- [ ] Server-side: object-oriented with prototypes; define at least `Player`, `Piece`, and `Game` classes
- [ ] Client: SPA built with a modern JS framework (React or Vue recommended); use Redux for state management
- [ ] No DOM manipulation libraries (e.g., jQuery), no Canvas, no SVG, no `<TABLE>` elements
- [ ] Layouts via CSS grid or flexbox
- [ ] Real-time communication via socket.io
- [ ] Server also serves `index.html`, `bundle.js`, and static assets via HTTP

### Game management
- [ ] Players join via URL: `http://<host>:<port>/<room>/<player_name>`
- [ ] First player to join a room becomes the host and controls game start/restart
- [ ] If host leaves, another player in the room becomes the new host
- [ ] No new players can join a game already in progress; they must wait for the next round
- [ ] Support multiple concurrent games

### Testing
- [ ] Unit test coverage ≥ 70% for statements, functions, and lines
- [ ] Unit test coverage ≥ 50% for branches

## Bonus

- [ ] Scoring system
- [ ] Persist player scores
- [ ] New game modes (e.g., invisible pieces, increased gravity)
- [ ] Explore Functional Reactive Programming (FRP) using a library like flyd
