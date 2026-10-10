# 2048

My educational project is a browser-based game called **2048**, written in JavaScript. The goal of the game is to move tiles around a 4 × 4 grid, merge identical numbers, and create a **2048** tile.

In this project, I implemented the game logic in a separate `Game` class and linked it to the interface via the DOM. Working on this game helped me practice working with arrays, managing state, and handling keyboard events.

[Play Online](https://freelinex.github.io/js-2048/)

## Features

- Move and merge tiles in four directions.
- Two random tiles appear at the start of the game.
- A tile with a value of 2 or 4 is added after a move that changes the board.
- Scoring: When tiles are merged, the value of the resulting tile is added to the score.
- Victory is achieved when a 2048 tile is obtained, and the game ends in defeat when no more moves are possible.
- Reset the game board and score using the **Restart** button.
- Tiles are colored according to their value.

## How to Play

1. Click **Start** to begin the game.
2. Use the **← ↑ → ↓** arrow keys on your keyboard. All tiles will move in the selected direction, and adjacent tiles with the same numbers will merge.
3. Create a **2048** tile before you run out of moves.

The **Restart** button resets the game. After resetting, press **Start** to begin a new game.

## Technologies

- **JavaScript** — game logic, events, and UI updates.
- **HTML** — markup for the game board and controls.
- **SCSS** — styles for the UI and tiles.
- **Parcel** and **@mate-academy/scripts** — project launch and build.
- **ESLint, Stylelint, and linthtml** — validation of JavaScript, styles, and HTML.

This project is based on a Mate Academy tutorial template.

## Running Locally

You'll need **Node.js** and **npm** to run this. The project's CI configuration uses Node.js 20.

```bash
git clone https://github.com/freelinex/js-2048.git
cd js-2048
npm install
npm start
```

Open the local address in your browser that appears in the terminal after the server starts.

## Commands

| Command | Purpose |
| --- | --- |
| `npm start` | Start the development server |
| `npm run build` | Build the project for publication |
| `npm run lint` | Check the code with linters |
| `npm run test:only` | Run tests using `mate-scripts test` |
| `npm test` | Run linters and the `test:only` test sequentially |
| `npm run deploy` | Deploy the project using `mate-scripts deploy` |

## Project Structure

```text
src/
├── index.html            # Game markup
├── modules/
│   └── Game.class.js     # State, moves, score, and result determination
├── scripts/
│   └── main.js           # Event handling and DOM updates
├── styles/
│   └── main.scss         # UI styles
└── images/
    └── reference.png     # Reference image
```

## License

This project is distributed under the [GPL-3.0](LICENSE) license.
