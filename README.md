# Pac-Man: Home Screen Edition

A browser-based Pac-Man clone where your phone's home screen is the maze. App icons are the dots — eat them all to advance to the next page.

## Play

Open `pacman_homescreen.html` in any modern browser. No build step, no dependencies.

## Screen capture wallpaper

On the start screen a **"📱 Use my screen as wallpaper"** button lets you play Pac-Man directly on top of your real screen or home screen.

| Platform | How it works |
|---|---|
| Desktop (Chrome / Edge / Firefox) | Click the button → pick a monitor or window in the browser's share picker → the live feed becomes the game background |
| Android (Chrome) | Tap the button → grant screen-share permission → navigate back to the game tab — your home screen plays live behind Pac-Man |
| iOS Safari | `getDisplayMedia` is not supported; the button is hidden and the game uses the default dark wallpaper |

When you stop sharing the game falls back to the original gradient automatically. A semi-transparent dark tint keeps all game elements readable over any wallpaper.

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
