# 🧠 Memory Card Matching Game

## Overview

This project is a browser-based Memory Card Matching Game developed using HTML, CSS, and JavaScript. Players flip cards to reveal hidden images and try to find matching pairs while keeping track of moves and elapsed time.

The game tests memory and concentration skills through an interactive and visually appealing interface.

---

## Features

- Interactive card-flipping animation
- Randomized card arrangement
- Move counter
- Game timer
- Matching pair detection
- Win condition checking
- Responsive user interface
- Start and Stop game controls

---

## Project Structure

```text
Memory-Game/
│
├── index.html
├── style.css
├── script.js
│
├── bee.png
├── bird.png
├── butterfly.png
├── cockatoo.png
├── tiger.png
├── monkey.png
├── tree.png
├── compass.png
├── capybara.png
├── waterfall.png
├── volcano.png
├── explorer.png
│
└── README.md
```

---

## Technologies Used

- HTML5
- CSS3
- JavaScript (ES6)

---

## Game Workflow

```text
Start Game
     │
     ▼
Generate Random Cards
     │
     ▼
Display Face-Down Cards
     │
     ▼
Player Selects First Card
     │
     ▼
Player Selects Second Card
     │
     ▼
Compare Cards
     │
 ┌───┴────┐
 │        │
Match   No Match
 │        │
 ▼        ▼
Keep     Flip Back
Open     After Delay
 │
 ▼
All Pairs Found?
 │
 ┌───┴────┐
 │        │
No       Yes
 │        │
 ▼        ▼
Continue  Display Win Message
```

---

## Game Components

### Timer

Tracks the total time taken by the player.

```javascript
setInterval(timeGenerator, 1000);
```

---

### Move Counter

Counts the number of attempts made.

```javascript
movesCounter();
```

---

### Card Generator

Randomly selects card pairs and shuffles them before displaying.

```javascript
generateRandom();
```

---

### Matching Logic

Checks whether two selected cards contain the same value.

```javascript
if(firstCardValue == secondCardValue)
```

---

### Win Detection

The game ends when all pairs are matched.

```javascript
if(winCount == Math.floor(cardValues.length / 2))
```

---

## User Interface

### Game Board

Displays all cards in a grid layout.

### Statistics Panel

Shows:

- Total Moves
- Elapsed Time

### Control Buttons

- Start Game
- Stop Game

---

## Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/memory-card-game.git

cd memory-card-game
```

---

## Running the Project

Simply open:

```bash
index.html
```

in any modern web browser.

No additional installation is required.

---

## Game Rules

1. Click Start Game.
2. Select a card to reveal its image.
3. Select another card.
4. If both cards match:
   - They remain open.
5. If they do not match:
   - They flip back after a short delay.
6. Continue until all pairs are matched.
7. Complete the game in minimum moves and time.

---

## Advantages

- Improves memory skills
- Enhances concentration
- Lightweight and fast
- Easy to customize
- Beginner-friendly JavaScript project

---

## Applications

### Educational Games

Memory training for students.

### Cognitive Skill Development

Improves recall and observation skills.

### Entertainment

Fun browser-based puzzle game.

### Web Development Learning

Understanding DOM manipulation and event handling.

---

## Future Enhancements

- Multiple difficulty levels
- Sound effects
- Leaderboard system
- Local storage for high scores
- Multiplayer mode
- Theme selection
- Mobile optimization

---

## Sample Card Categories

```text
Bee
Bird
Butterfly
Cockatoo
Tiger
Monkey
Tree
Compass
Capybara
Waterfall
Volcano
Explorer
```

---

## Results

The game successfully generates randomized card layouts, tracks player performance through move counts and timers, and provides an engaging memory-testing experience using pure JavaScript.

---

## Author

**Udata Lekhana Surya Bhanu**

Mini Project – Memory Card Matching Game using HTML, CSS, and JavaScript

---

## License

This project is intended for academic and educational purposes.
