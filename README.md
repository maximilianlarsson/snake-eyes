# Snake Eyes

A polished browser version of **Snake Eyes**, built as a single self-contained HTML file.

It supports any number of players, animated 2D dice, sound effects, and a full-screen snake flash when a player rolls double ones.

## Features

- Any number of players
- Mobile-friendly layout
- Animated 2D pip dice
- Sound effects for roll, hold, bad roll, snake eyes, and win
- Full-screen snake emoji flash on snake eyes
- No dependencies
- No build step
- Runs entirely in the browser

## Game rules

Each player takes turns rolling **two dice**.

- If **neither die is 1**, the sum is added to the player's **running total for the current turn**
- The player can then choose to:
  - **Roll again** to try to build a higher turn total
  - **Hold** to bank the turn total into their permanent score
- If **exactly one die is 1**, the player's **turn total becomes 0** and the turn ends
- If the roll is **double ones**, that is **Snake Eyes**
  - The player loses **all banked points**
  - The turn ends immediately
- First player to reach **100 points or more** wins

## Controls

### Setup screen

Enter one player name per line, then press **Start Game**.

### In game

- **Roll**: roll both dice
- **Hold**: bank the current turn total
- **New Game**: return to the player selection screen with the last player list still pre-filled
- **Reset**: reset the player list back to the default sample names
- **Toggle Sound**: turn sound effects on or off

### Keyboard shortcuts

- `R` = Roll
- `H` = Hold

## Files

- `snake-eyes.html` — the game
- `README.md` — project overview and usage

## Run locally

No installation is needed.

Open the HTML file directly in a browser:

```bash
open snake-eyes.html
```

Or just double-click the file.

## iPhone / iPad notes

For best results on iOS:

- Open the file in **Safari**
- Avoid the Files app preview mode for interactive HTML
- Tap once anywhere if sound does not start immediately, since iOS may require a user interaction before enabling audio

## GitHub Pages

This project can be hosted directly with GitHub Pages because it is a static site.

A simple structure is enough:

```text
/
├── index.html
└── README.md
```

To publish it, rename `snake-eyes.html` to `index.html` and push it to your repository.

## Customization ideas

Easy upgrades you could add later:

- Exact-100 win rule
- Score history log
- Player colors or avatars
- Confetti on win
- Dark/light theme switch
- Persistent saved settings with localStorage

## License

Use it freely for personal projects or adapt it for your own game night.
