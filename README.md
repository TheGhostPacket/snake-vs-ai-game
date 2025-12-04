# 🐍 Snake vs AI

A modern, browser-based Snake game where you compete against an intelligent AI opponent. Built with vanilla JavaScript, HTML5 Canvas, and CSS3.

![Game Preview](preview.png)

## 🎮 Play Now

Simply open `index.html` in any modern web browser — no installation required!

## ✨ Features

- **AI Opponent**: Compete against a pathfinding AI that adapts to different difficulty levels
- **4 Difficulty Modes**:
  - 🟢 **Easy** — Casual AI with 30% random moves
  - 🟡 **Medium** — Smart AI with 15% random moves
  - 🔴 **Hard** — Expert AI with 5% random moves
  - ⚫ **Impossible** — Perfect AI, always optimal moves
- **Wrap-Around Edges**: Snakes teleport to the opposite side when hitting walls
- **Real-Time Stats**: Track game time, scores, snake lengths, and food eaten
- **Responsive Design**: Works on desktop and mobile devices
- **Touch Controls**: On-screen D-pad for mobile play
- **Clean UI**: Modern dark theme with smooth animations

## 🕹️ Controls

| Key | Action |
|-----|--------|
| `↑` `W` | Move Up |
| `↓` `S` | Move Down |
| `←` `A` | Move Left |
| `→` `D` | Move Right |
| `Space` | Pause/Resume |
| `R` | Restart Game |

## 🧠 How the AI Works

The AI uses a scoring system to evaluate each possible move:

1. **Safety Check**: Avoids collisions with itself and the player
2. **Food Seeking**: Calculates Manhattan distance to food
3. **Space Analysis**: Uses flood-fill to estimate available movement space
4. **Player Avoidance**: On harder difficulties, keeps distance from the player's head

The difficulty level determines how often the AI makes optimal vs random decisions.

## 🏆 Win Conditions

- **You Win**: AI crashes into itself or you have a higher score on collision
- **AI Wins**: You crash into yourself or AI has a higher score on collision
- **Tie**: Both snakes crash simultaneously with equal scores

## 🛠️ Tech Stack

- HTML5 Canvas for rendering
- Vanilla JavaScript (ES6+)
- CSS3 with CSS Variables
- Font Awesome icons
- No external dependencies

## 📁 Project Structure

```
snake-vs-ai/
├── index.html    # Complete game (single file)
└── README.md     # This file
```

## 🚀 Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/snake-vs-ai.git
   ```

2. Open `index.html` in your browser

That's it! No build process or dependencies needed.

## 📱 Mobile Support

The game automatically detects mobile devices and displays touch controls. The canvas scales responsively to fit smaller screens.

## 🎨 Customization

Colors and styling can be easily modified through CSS variables in the `:root` selector:

```css
:root {
    --player-color: #4ade80;  /* Green */
    --ai-color: #f59e0b;      /* Orange */
    --food-color: #ef4444;    /* Red */
}
```

## 📄 License

MIT License — feel free to use, modify, and distribute.

## 🤝 Contributing

Contributions are welcome! Feel free to:

- Report bugs
- Suggest new features
- Submit pull requests

---

**Built by [TheGhostPacket](https://theghostpacket.com)** | Part of the ShieldStack Technologies portfolio
