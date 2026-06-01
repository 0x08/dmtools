# ⚔️ Ben's Encounter Tracker

A lightweight, blazing-fast, pure frontend web application designed for Dungeon Masters running high-stakes tabletop RPG combat. It handles initiative order with active turn management, tracks monster hit points with instant math modifiers, and saves a persistent library of creatures right inside your browser's native memory.

No servers, no databases, no complex setup. Just open the HTML file and play.

---

## 🚀 Quick Start

1. **Download the code**: Save the `dm_tracker.html` file to your local computer.
2. **Launch**: Double-click the file to open it in any modern web browser (Chrome, Firefox, Edge, Safari).
3. **Play**: Bookmark it for immediate access behind your DM screen.

---

## 🛠️ Key Features

### 1. Active Turn & Round Manager

- **Next / Previous Cycling**: Use the **Next ▶** and **◀ Previous** buttons to cycle through characters seamlessly. The tracker automatically loops cleanly from the bottom of the order back to the top (and vice versa).
- **Visual Turn Frame**: The combatant whose turn it is instantly highlights with an amber glow, a pulsing `ACTIVE` banner, and a `⚔️` icon so you can see who is acting at a glance.
- **Smart Death Skipping 🤖**: When a monster hits `0` HP or lower, the turn tracker will automatically skip past them during turn cycles, ensuring you only pause on combatants who are actually conscious.

### 2. Streamlined Encounter Entry

- **Instant Re-focus**: Pressing Enter to add a combatant automatically snaps your typing cursor straight back into the **Name** field, allowing you to queue up a whole group of enemies entirely from your keyboard.
- **Auto-Select Fields**: Clicking into any **Initiative** score or **HP** field instantly highlights the entire value, allowing you to overwrite or modify text without wasting time hitting backspace.
- **Auto-Numbering Duplicates**: Adding multiple identical monsters (e.g., clicking your "Goblin" template 4 times) automatically decorates them as `Goblin #1`, `Goblin #2`, etc.

### 3. Integrated Collapsible Bestiary

- **Accordion View**: The Library / Bestiary module stays neatly collapsed by default to keep your screen tidy, unfolding with a single click when you need to spawn reinforcements.
- **One-Click Spawning**: Click any profile card inside your library to instantly drop that character or creature into the active initiative order with their default stats.
- **Local Storage Save**: Creatures added to your library are committed to HTML5 `localStorage`. They will stay right there safely even if you close your laptop or clear your browser cache.

---

## ⌨️ Shortcuts & Math Engine

- **In the Active Initiative List**:
  - Click an HP box, type `-Value` (e.g., `-22`) or `+Value` (e.g., `+10`), and press **Enter** to let the engine calculate damage/healing dynamically.
  - Type a flat number (e.g., `45`) and hit **Enter** to completely overwrite their current HP state.
  - Clicking **Sort 🎲** will arrange combatants from highest initiative to lowest and automatically lock the active turn to the top of the round.
- **In the Bestiary Creator**:
  - Leaving Max HP at `0` automatically registers a profile as a Player Character (`🛡️`). Setting it above `0` registers them as a Monster (`😈`).

---

## 🔒 Security & Privacy

- **100% Offline**: This application doesn't collect analytics, communicate with cloud data silos, or make external API requests. Your campaign notes and character names remain strictly private to your computer.
