

# 🚜 Pixel Bridge Runner

> A retro-style pixel adventure game built using pure **HTML, CSS, and JavaScript** featuring **100 handcrafted levels** and smooth arcade gameplay.

<img width="959" height="419" alt="image" src="https://github.com/user-attachments/assets/d0460619-66d5-4c78-9ad0-f897cfddbbaa" />

<img width="959" height="416" alt="image" src="https://github.com/user-attachments/assets/d4bb0602-7d6d-47de-8145-602f717aad38" />




---

## 🎮 About the Game

**Pixel Bridge Runner** is a lightweight browser game where players control a pixel truck and navigate through bridges, platforms, and obstacles.

Designed with a **minimal pixel art aesthetic**, the game focuses on:

* 🎯 Precision movement
* 🧠 Timing & strategy
* 🚀 Increasing difficulty across 100 levels
* ⚡ Instant play in the browser (no install required)

Perfect for quick fun or casual challenges!

---
The logic of "Where are the assets if there is no database?" using a real-life analogy.

The Core Concept: The "Packed Suitcase"
Think of a traditional website (like Amazon) as a Restaurant.

You (The Browser): Sit at a table and order food.

The Waiter (API): Takes your order to the kitchen.

The Kitchen (Backend/Database): Cooks the specific meal you asked for (fetches data) and sends it back.

If the kitchen closes (offline), you don't get food.

Your game is different. It is like a Lunchbox.

The Server: Is just the delivery driver. They hand you the entire lunchbox (the game files).

You (The Browser): Open the box. Everything you need—the sandwich, the apple, the napkin—is already inside.

Once you have the lunchbox, you don't need the driver or the kitchen anymore. You can eat (play) even in a bunker.

Technical Breakdown: How the "Lunchbox" is Packed
In your specific game (Drive Mad), the "Lunchbox" consists of three specific files that work together. Here is the logic of each:

1. index.html (The Instructions)
Real Life: This is the note inside the lunchbox that says, "Eat the sandwich first, then the apple."

Logic: It tells the browser which files to load and in what order. It sets up the screen (canvas) where the game will be displayed.

2. index.wasm.js (The Engine / The Brain)
Real Life: This is you, the eater. It knows how to eat. It knows the rules: "Chew before swallowing."

Logic: This contains the game logic (physics, collisions, win/loss states). It was likely written in a language like C++ or C# and compiled into WebAssembly. It doesn't hold the pictures, it holds the rules.

3. index.data.js (The Assets / The Food)
Real Life: This is the sandwich, the apple, and the juice box.

Logic: This is the most important part of your friend's question. This file is a Virtual File System.

Instead of storing images (car.png) and sounds (crash.mp3) on a server database, the developers took all those files and converted them into one giant block of text/code inside this .js file.

When the game starts, the browser reads this file and "unpacks" it into memory (RAM).

The "Trick": The game thinks it is reading files from a hard drive, but it's actually just reading from this memory blob that the browser downloaded.

The "No Database" Logic Flow
Here is exactly what happens when you click "Play":

Download: Your browser downloads index.data.js (The packed assets).

Mounting: The WebAssembly code creates a fake hard drive in your browser's RAM.

Unpacking: It takes the data from index.data.js and places the "virtual" images and sounds onto that fake hard drive.

Playing: When the car crashes, the game code says "Play sound crash.mp3". It doesn't ask a server; it asks the fake hard drive in your RAM.

---

## ✨ Features

* 🧩 100 unique levels
* 🎨 Retro pixel graphics
* ⚡ Smooth animations
* ⌨️ Keyboard controls
* 🌐 Runs directly in browser
* 📱 Lightweight & fast
* 🧠 Progressive difficulty

---

## 🛠️ Tech Stack

| Technology                  | Purpose                       |
| --------------------------- | ----------------------------- |
| **HTML5**                   | Game structure & canvas       |
| **CSS3**                    | Styling & pixel visuals       |
| **JavaScript (Vanilla JS)** | Game logic, physics, controls |
| **Canvas API**              | Rendering & animations        |
| **index.data.js**           | The Assets                    |
| **index.wasm.js**           | Engine                        |

> No frameworks. No libraries. Pure JavaScript game engine.

---

## 📂 Project Structure

```
📦 Pixel-Bridge-Runner
 ┣ 📜 index.html   → Complete game code (HTML + CSS + JS)
 ┣ 📜 README.md
 ┗ 📜 assets/      → images/sprites (optional)
```

> All game logic is inside `index.html` for simplicity.

---

## ▶️ How to Play

### Run locally

```bash
git clone https://github.com/your-username/pixel-bridge-runner.git
cd pixel-bridge-runner
open index.html
```

or just **double-click index.html**

---

## 🎮 Controls

| Key | Action        |
| --- | ------------- |
| ← → | Move          |
| ↑   | Jump          |
| R   | Restart level |

---

## 🚀 Live Demo : https://detailed-coral-qyq2m13xdp.edgeone.app/

👉 Add your deployed link here
Example:

```
https://your-username.github.io/pixel-bridge-runner/
```

---

## 📸 Screenshots

Add screenshots like:

```
<img width="959" height="410" alt="image" src="https://github.com/user-attachments/assets/d62bccd8-8725-4979-9994-f3f40de07535" />

<img width="959" height="415" alt="image" src="https://github.com/user-attachments/assets/12451c31-8a25-48a2-8d95-93db6b4e1917" />

```

---

## 🎯 Learning Goals

This project helped practice:

* DOM manipulation
* Game loops
* Collision detection
* Physics basics
* Canvas rendering
* Vanilla JS architecture

---

## 💡 Future Improvements

* 🔊 Sound effects
* 🎵 Background music
* 💾 Save progress
* 🏆 Score system
* 📱 Mobile controls
* Multiplayer mode

---

## 🤝 Contributing

Pull requests are welcome!
Feel free to fork and improve the game.


## ⭐ Support

If you like this project:

⭐ Star the repo
🍴 Fork it
🧑‍💻 Share with friends


