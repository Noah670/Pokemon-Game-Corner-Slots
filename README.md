# 🎰 Pokémon Game Corner Slots

A mobile-friendly, single-file recreation of the classic Pokémon Game Corner from Generation 1-3 (FireRed, LeafGreen, Emerald), featuring slot machines, town exploration, and a prize redemption system.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Static](https://img.shields.io/badge/static-HTML%2FJS-orange.svg)
![Mobile](https://img.shields.io/badge/platform-mobile--first-brightgreen.svg)

## 🌐 Live Preview (GitHub Pages)

Once GitHub Pages is enabled, your live site will be available here:

```
https://<your-github-username>.github.io/Pokemon-Game-Corner-Slots/
```

## ✨ Features

### 🎮 Three Game Modes
- **Town Exploration** - Navigate through Celadon City using arrow keys or touch controls
- **Slot Machine Casino** - Classic 3-reel slot machine with authentic Pokémon Game Corner mechanics
- **Prize Corner** - Redeem your coins for TMs and rare Pokémon

### 🎯 Core Gameplay
- **Authentic Slot Mechanics** - Multiple symbol types with varying payouts
- **Coin Economy** - Start with 500 coins, bet 10-100 coins per spin
- **Prize System** - Collect TMs (Ice Beam, Thunderbolt, Flamethrower) and Pokémon (Porygon, Dratini, Abra)
- **Town Map** - 10x10 grid-based navigation system
- **Progressive Stats** - Track total wins and coin balance

### 📱 Mobile Optimized
- Touch-friendly controls
- Responsive design (max-width: 448px)
- Smooth animations and transitions
- Works on iOS and Android browsers

## 🚀 Quick Start

### Run locally

Open the game directly in your browser:

```bash
# From the repo root
open index.html
```

## 🛠️ Technology Stack

- **Frontend**: React 18 (CDN)
- **Styling**: Tailwind CSS (CDN)
- **Language**: JavaScript (ES6+)

## 📁 Project Structure

```
Pokemon-Game-Corner-Slots/
├── index.html        # Single-file game (HTML + React + Tailwind via CDN)
└── README.md
```

## 🎮 How to Play

### Town Navigation
1. **Keyboard**: Use arrow keys (↑ ↓ ← →) to move your character
2. **Touch**: Tap directional buttons on mobile
3. **Locations**:
   - 🎰 Game Corner - Enter the casino
   - 🏪 Prize Shop - Redeem coins for prizes
   - 🏠 Houses - Decorative buildings
   - 🌳 Trees - Impassable terrain

### Slot Machine
1. **Select Bet**: Choose 10, 25, 50, or 100 coins
2. **Spin**: Tap the SPIN button
3. **Win Conditions**:
   - **7-7-7**: 100x bet (jackpot!)
   - **💎-💎-💎**: 50x bet
   - **🔔-🔔-🔔**: 30x bet
   - **⭐-⭐-⭐**: 20x bet
   - **🍒-🍒-🍒**: 15x bet
   - **BAR-BAR-BAR**: 10x bet
   - **🍒-🍒-?**: 5x bet (cherry bonus)

### Prize Corner
- **TM13 Ice Beam** - 4,000 coins
- **TM24 Thunderbolt** - 4,000 coins
- **TM35 Flamethrower** - 4,000 coins
- **Porygon** - 9,999 coins (rarest prize!)
- **Dratini** - 2,800 coins
- **Abra** - 120 coins

## 🔧 Configuration

### Adjusting Starting Coins
Edit the initial state in `index.html`:

```javascript
const [coins, setCoins] = useState(500); // Change 500 to your desired amount
```

### Modifying Payout Rates
Update the `checkWin` function:

```javascript
if (result[0] === "7") winAmount = bet * 100; // Adjust multipliers here
```

### Adding New Prizes
Extend the `prizeList` array:

```javascript
const prizeList = [
  { name: "Your Prize", cost: 1000, icon: "🎁" },
  // Add more prizes...
];
```

## 🎨 Customization

### Color Scheme
The app uses Tailwind CSS utility classes. Modify colors in JSX:

```javascript
// Change casino background gradient
<div className="bg-gradient-to-b from-red-700 to-red-900">
```

### Map Design
Edit the `townMap` array to create custom layouts:

```javascript
const townMap = [
  ['🌳', '🌳', '🏠', '🌳'],
  // Customize your map...
];
```

## 🚀 Deployment

### Deploy to GitHub Pages
1. Push this repository to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose:
   - **Source**: Deploy from a branch
   - **Branch**: `main` (or your default branch)
   - **Folder**: `/ (root)`
4. Save, then wait 1-2 minutes for the site to publish.

Your site will be available at:

```
https://<your-github-username>.github.io/Pokemon-Game-Corner-Slots/
```

## 🐛 Known Issues & Roadmap

### Current Limitations
- No sound effects (placeholder for future implementation)
- In-memory state only (coins reset on page refresh)
- Limited to 6 prize types

### Planned Features
- [ ] Persistent storage using localStorage
- [ ] Sound effects and background music
- [ ] Additional mini-games (Card Flip, Roulette)
- [ ] Multiplayer leaderboards
- [ ] Daily login bonuses
- [ ] Achievement system
- [ ] Animated sprite characters
- [ ] Multiple save slots

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Code Style
- Use ES6+ features
- Follow React best practices
- Maintain mobile-first responsive design
- Comment complex logic

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Inspired by Pokémon FireRed, LeafGreen, and Emerald Game Corners
- Game Freak and Nintendo for the original Pokémon games
- The Pokémon community for keeping the nostalgia alive

## 📞 Support

- **Issues**: [GitHub Issues](https://github.com/yourusername/pokemon-game-corner/issues)
- **Discussions**: [GitHub Discussions](https://github.com/yourusername/pokemon-game-corner/discussions)

## 🎯 Performance

- Instant load (single HTML file)
- 60 FPS animations
- Mobile-optimized touch events
- Minimal re-renders with React hooks

---

**Made with ❤️ for Pokémon fans everywhere**

⭐ Star this repo if you enjoyed playing!
