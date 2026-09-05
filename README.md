# Pac-Man: Home Screen Edition

A browser-based Pac-Man clone where your phone's home screen is the maze. App icons are the dots — eat them all to advance to the next page.

## Play

Open `pacman_homescreen.html` in any modern browser. No build step, no dependencies.

## Use your real desktop icons

The **"🖥️ Use my desktop icons"** button lets you play with your own files as the app icons instead of the built-in list.

| Browser | How it works |
|---|---|
| Chrome / Edge (desktop & Android) | Opens a folder picker (File System Access API) — point it at your Desktop and every file inside becomes an icon in one shot, sorted alphabetically to approximate your normal icon layout |
| Firefox / Safari | Falls back to a classic multi-file picker (select one or more files) |
| Any browser | You can also drag and drop files directly onto the game canvas |

Image files are drawn as real thumbnails; everything else gets a color/emoji icon based on its file type. Browsers have no API to read the actual on-screen (x, y) position of your desktop icons, so the imported layout is an approximation (alphabetical order), not a pixel-perfect copy of your desktop.

## Full-screen mode

Tap the **⛶** button in the top-right corner to play full-screen (uses the browser's Fullscreen API). Tap it again (now showing **⤢**) to exit. The button is hidden automatically on browsers that don't support it (e.g. iOS Safari before 16.4).

## How to play

- **Eat all the app icons** on each of the 3 home screen pages to win
- **Avoid the ghosts** — they'll cost you a life
- **Power pellets** (⚡) appear in the four corners — grabbing one makes ghosts vulnerable and edible for 8 seconds
- You start with **3 lives**

## Controls

| Input | Action |
|---|---|
| Arrow keys / WASD | Move |
| On-screen D-pad | Move (mobile) |
| Swipe on canvas | Move (touch) |
| Space / Enter | Start / restart |
| Tap canvas | Start / restart |

## Ghost personalities

- **Blinky** (red) — direct chaser, always targets Pac-Man
- **Pinky** (pink) — ambusher, targets 4 cells ahead of Pac-Man
- **Inky** (cyan) — flanker, uses Blinky's position as a reference point
- **Clyde** (orange) — wanderer, chases when far away, retreats when close

## Levels

Each of the 3 levels is a new "home screen page" with a different set of app icons. Ghosts get slightly faster with each level.
