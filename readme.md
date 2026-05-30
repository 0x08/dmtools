# ⚔️ DM Encounter & Initiative Tracker

A lightweight, blazing-fast, pure frontend web application designed for Dungeon Masters running D&D or other tabletop RPGs. It handles initiative order, tracks monster hit points with instant math modifiers, and saves a local bestiary using your browser's native memory.

No servers, no databases, no installation required. Just open the HTML file and play.

---

## 🚀 Quick Start

1. **Download the code**: Save the `dm_tracker.html` file to your computer.
2. **Launch**: Double-click the file to open it in any web browser (Chrome, Firefox, Edge, Safari).
3. **Play**: Bookmark it for instant access behind your DM screen.

---

## 🛠️ Key Features

### 1. Dynamic Initiative Tracking
* Input character or monster names, add their rolled initiative, and click **Sort 🎲** to instantly arrange combatants from highest to lowest.
* Modify initiative scores directly inside the live table if a creature's order changes mid-round.

### 2. Smart HP Tracker (Monsters Only)
* **Relative Math Parsing**: Instead of doing mental math, click a monster's HP box, type a modifier like `-11` or `+5`, and press **Enter**. The tool updates the math automatically.
* **Auto-Highlight**: Clicking or tapping an HP input automatically selects the entire text, letting you update health scores without pressing backspace.
* **Visual Death States**: When a monster hits 0 HP or lower, its name turns gray, a `💀` icon replaces its avatar, and its health bar strikes through.

### 3. Integrated Library & Bestiary
* **One-Click Spawning**: Tap any profile card in your Bestiary to instantly throw that creature into the active initiative order.
* **Auto-Numbering Duplicates**: Spawning multiple identical creatures (e.g., clicking "Goblin" 4 times) automatically names them `Goblin #1`, `Goblin #2`, `Goblin #3`, and `Goblin #4`.
* **Persistent Memory**: Player Characters and Monsters are saved directly to your browser's `localStorage`. They remain there safely even if you close the browser or restart your computer.

---

## ⌨️ Shortcuts & Tips

* **In the Main Tracker**:
  * Type `-Value` or `+Value` in the HP box and hit **Enter** to modify hit points.
  * Type a flat number (e.g., `25`) and hit **Enter** to overwrite HP completely.
* **In the Bestiary Creator**:
  * Type a Name, type a Max HP value, and press **Enter** to rapidly build your library before game night. Leaving HP at `0` automatically registers the profile as a Player Character.

---

## 🔒 Privacy & Architecture

* **Zero Tracking**: This app does not connect to any server, track analytics, or store cookies. Your campaign data never leaves your machine.
* **Storage Tech**: It uses HTML5 `localStorage` to save your Bestiary template variables. 
* **Styling**: Built utilizing vanilla JavaScript and a Tailwind CSS CDN package for a native, eye-strain-free dark mode.
