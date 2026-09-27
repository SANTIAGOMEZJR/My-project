# Pet Shield

Pet Shield is a cute 2D HTML5 survival game built with Phaser. Draw a magical shield around the pet and protect it from incoming bees for as long as possible.

## Play

Open the GitHub Pages link for this repository on a phone or desktop browser. The game is designed primarily for portrait mobile screens.

## How to Play

- Press **START** to begin.
- Drag your finger or mouse to draw a protective line.
- Bees that touch the shield are blocked.
- Drawing a new shield causes the previous shield to fade away.
- Survive as long as possible and beat your best score.
- The animated tutorial is non-blocking and can be skipped by interacting immediately.

## Features

- Infinite survival mode
- Touch and mouse drawing controls
- 360-degree freeform protection
- Animated onboarding tutorial
- Responsive full-screen mobile layout
- Local best-score storage
- Fully offline Phaser runtime and game assets

## Technology

- HTML5
- JavaScript
- Phaser 3.88.2
- Canvas/WebGL

## Run Locally

The game uses relative asset paths. For the most reliable local testing, serve the repository with a small static web server and open `index.html`.

For example, with Python installed:

```bash
python -m http.server 8080
```

Then visit:

```text
http://localhost:8080/
```

## Project Structure

```text
.
|-- index.html
|-- assets/
|   |-- manifest.js
|   |-- background/
|   |-- characters/
|   |-- effects/
|   `-- ui/
`-- lib/
    `-- phaser.min.js
```

## Asset Notice

The game artwork and visual assets are original project assets and are not licensed for reuse unless permission is granted separately.

