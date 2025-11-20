# Flappy HTML5 Bird 🐦

A faithful HTML5 recreation of the classic Flappy Bird game, built with CoffeeScript, jQuery, and SCSS.

![Game Preview](cover.png)

## Features

- 🎮 Classic Flappy Bird gameplay
- 🎨 Original game graphics and animations
- 📱 Responsive canvas-based rendering
- ⚡ Smooth animations using CSS keyframes
- 🏆 Score tracking with high score system

## Tech Stack

- **HTML5** - Game structure
- **CoffeeScript** - Game logic (475 lines)
- **SCSS/CSS** - Styling and animations (380 lines)
- **jQuery** - DOM manipulation
- **Canvas/Sprites** - Game graphics

## Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- Modern web browser (Chrome, Firefox, Safari, or Edge)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/ben7th/flappy-html5-bird.git
cd flappy-html5-bird
```

2. Install dependencies:
```bash
npm install
```

## Running the Game

### Option 1: Using npm (Recommended)

Start the development server:
```bash
npm start
```

This will automatically open the game in your default browser at `http://localhost:8080`

### Option 2: Using npm dev mode

For development with cache disabled:
```bash
npm run dev
```

### Option 3: Direct file access

You can also open `index.html` directly in your browser, but some browsers may restrict local file access. Using the http-server method above is recommended.

### Option 4: Using Python's built-in server

If you don't want to install npm dependencies:
```bash
# Python 3
python -m http.server 8080

# Python 2
python -m SimpleHTTPServer 8080
```

Then open `http://localhost:8080` in your browser.

## How to Play

1. Click or press any key to start the game
2. Click or press any key to make the bird flap its wings
3. Avoid the pipes and the ground
4. Try to get the highest score possible!

## Project Structure

```
flappy-html5-bird/
├── index.html              # Main HTML file
├── cover.png               # Game preview image
├── ui/
│   ├── bird.css            # Compiled CSS (generated from SCSS)
│   ├── bird.scss           # Game styles and animations
│   ├── bird.js.coffee      # Game logic in CoffeeScript
│   ├── document.css        # Document styles
│   ├── document.scss       # Document SCSS source
│   ├── images/             # Game sprites and graphics
│   │   ├── bird.png
│   │   ├── pipe_*.png
│   │   ├── stage_*.png
│   │   └── ...
│   └── lib/                # External libraries
│       ├── coffee-script.js
│       └── jquery-2.1.0.min.js
├── package.json            # Node.js dependencies
└── README.md              # This file
```

## Development

The game uses CoffeeScript which is compiled in the browser using `coffee-script.js`. If you want to modify the game logic:

1. Edit `ui/bird.js.coffee`
2. Refresh your browser - the CoffeeScript compiler will handle the compilation automatically

For styling changes:

1. Edit `ui/bird.scss` or `ui/document.scss`
2. Compile SCSS to CSS using your preferred method (sass, node-sass, etc.)
3. Or edit the compiled `.css` files directly for quick changes

