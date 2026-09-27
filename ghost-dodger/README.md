# 👻 Ghost Dodger

**Ghost Dodger** is a fast-paced, highly addictive web-based survival game built entirely with HTML5 Canvas, CSS, and Vanilla JavaScript. Your goal is simple but challenging: survive as long as possible by dodging the relentless rain of falling ghosts! 

Whether you're looking for a quick break or aiming to beat your personal best, Ghost Dodger delivers instant fun directly in your browser.

---

## 🏆 Why Ghost Dodger? (Pros vs. Existing Systems)

When compared to other browser games or heavy standalone titles, Ghost Dodger stands out for its simplicity, speed, and privacy:

- **Zero Dependencies & Zero Installation:** Unlike games built with heavy engines (Unity, Unreal) or complex JS frameworks (React, Phaser), Ghost Dodger is purely Vanilla. No `npm install`, no complex build steps, and no downloading large executables.
- **Blazing Fast Load Times:** With a microscopic footprint, the game loads instantly on any internet connection. No loading screens, just instant gameplay.
- **Privacy First (Local Storage):** Your high scores, unlocked skins, and collected coins are saved locally on your device. There are no accounts to create, no servers tracking your behavior, and absolutely no intrusive ads or microtransactions.
- **Offline Playability (PWA):** Install the game on your device as a Progressive Web App and play it anytime, anywhere, even without an internet connection.
- **Clean & Educational Codebase:** The entire game runs from a single HTML file with elegantly structured JavaScript. It serves as a perfect learning resource for developers wanting to understand game loops, collision detection, and HTML5 Canvas mechanics.
- **Cross-Platform Accessibility:** Works seamlessly on any modern operating system (Windows, macOS, Linux, iOS, Android) with a web browser.

---

## ✨ Key Features

- **🛒 In-Game Shop (New!):** Use collected coins to purchase and permanently unlock premium skins (like 👽, 🤖, 🦸‍♂️, 🦄). Unlocks are saved across sessions!
- **👹 Epic Boss Fights (New!):** Every 3 levels, normal ghost spawning stops and you face off against a giant Boss Ghost. Survive the barrage of projectiles and automatically fire back to defeat it for a massive coin bonus.
- **🎶 Web Audio SFX (New!):** Immerse yourself in the action with dynamically generated, 8-bit retro sound effects for coins, power-ups, hits, and boss battles (powered purely by the browser's native AudioContext).
- **🌟 Score Combo Multiplier (New!):** Grab coins quickly in succession to build up your combo multiplier (up to 5x) for massive wealth accumulation.
- **🌈 Dynamic Biome Themes (New!):** The background dynamically changes depending on the level to keep things fresh. Experience unique weather effects like rain, fog, starry space, and floating embers!
- **Evolving Enemy Types:** Face new challenges as you level up! Start with normal falling ghosts, progress to swaying **Zig-Zag Ghosts** (👻), and try to outrun aggressive **Chaser Ghosts** (💀) that track your movements.
- **Interactive Powerup System:** Strategic items drop from the sky to help you survive:
  - 🛡️ **Shield:** Grants temporary immunity against collisions.
  - 🐢 **Slow Motion:** Temporarily reduces the speed of the falling ghosts.
  - 🧲 **Magnet (New!):** Pulls all nearby coins directly to you!
  - ❄️ **Time Freeze (New!):** Completely stops ghost movement for a few seconds.
  - 🍄 **Shrink Potion (New!):** Shrinks your character, giving you a tiny hitbox to dodge through tight spaces.
- **Score Sharing:** Boast to your friends by easily sharing your high score and difficulty level using the native Share Score button at the end of a round.
- **Multiple Selectable Difficulties:** Choose between Easy, Medium, and Hard right from the start menu to tailor the initial ghost speed to your skill level.
- **Seamless Pause Functionality:** Need a quick break? Hit the `Esc` key to pause the action without losing your progress.

---

## 🎮 How to Play

- **Movement:** Use the **Left** (⬅️) and **Right** (➡️) arrow keys to move your character horizontally across the screen.
- **Objective:** Avoid the falling ghosts (👾). If a ghost touches you (and you have no shield), it's Game Over!
- **Boss Fights:** Dodge the red projectiles. Your character automatically shoots upward at the boss.
- **Powerups:** Intercept the falling powerups to gain temporary advantages.
- **Pause:** Press the **Escape (Esc)** key at any point to pause or unpause the game.

---

## 🚀 Getting Started

Getting the game running on your machine is incredibly simple. 

1. **Clone or Download** this repository to your local machine.
2. Navigate to the project folder.
3. Simply open the `Index.html` file in your preferred modern web browser. *(Note: To test the PWA Offline functionality specifically, you will need to serve the folder via a local web server, e.g., `python -m http.server 8000`).*
4. *That's it!* Select your difficulty, choose a skin, and start dodging!

---

## 🛠️ Technologies Used

Ghost Dodger was crafted to be as lightweight and native as possible:

- **HTML5 (Canvas API):** Provides the foundational structure and the high-performance rendering context for the game loop, sprites, and dynamic weather backgrounds.
- **Web Audio API:** Used to dynamically generate retro synthesizer sound effects without needing external `.mp3` or `.wav` files.
- **CSS3:** Used for the sleek UI overlays, modern gradients, typography, and smooth CSS animations (like the fade-in screens).
- **Vanilla JavaScript (ES6+):** Drives the core game loop, entity management, collision detection algorithms, event handling, and HTML5 `localStorage` integration.
- **Service Workers:** Powers the Progressive Web App (PWA) capabilities, allowing the game to cache assets and be played entirely offline.

---
## 🤝 Contributing

This project is open-source and highly extensible! If you want to add new powerups, more enemy types, sound effects, or mobile touch controls, feel free to fork the repository and submit a pull request.
