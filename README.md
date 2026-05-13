# Simon Game 🎮

A browser-based implementation of the classic **Simon** memory game, built with HTML, CSS, and JavaScript (jQuery).

## How to Play

1. Open `index.html` in your browser.
2. Press any key **or** click the **Start** button to begin.
3. Watch the sequence of colored buttons that light up.
4. Repeat the sequence by clicking the buttons in the same order.
5. Each round adds one more step to the sequence — how far can you go?

## Game Rules

- The game generates a random color sequence and adds one new color each level.
- You must reproduce the full sequence correctly to advance.
- A wrong click ends the game — the screen flashes red and a "Game Over" message appears.
- Press any key or click **Start** to restart after a game over.

## Project Structure

```
simon-game/
├── index.html      # Game layout and structure
├── styles.css      # Styling and animations
├── game.js         # Game logic (jQuery)
└── sounds/         # Audio files for each button and wrong answer
    ├── red.mp3
    ├── blue.mp3
    ├── green.mp3
    ├── yellow.mp3
    └── wrong.mp3
```

## Technologies Used

- **HTML5** — page structure
- **CSS3** — styling, button animations, game-over flash
- **JavaScript (ES5)** — game logic
- **jQuery 3.7.1** — DOM manipulation and event handling
- **Google Fonts** — *Press Start 2P* retro font

## Running Locally

No build tools or dependencies required. Just open `index.html` directly in any modern browser:

```bash
# Option 1: Open directly
open index.html

# Option 2: Serve with a simple HTTP server
npx serve .
# or
python -m http.server 8000
```

> **Note:** Some browsers block local audio autoplay. If sounds don't play, try serving the files via a local HTTP server instead of opening the file directly.

## Features

- Progressive difficulty — sequence grows by one each level
- Visual feedback — buttons flash when activated
- Audio feedback — each button has a unique sound
- Game over animation — screen flashes red on a wrong answer
- Keyboard or button start support