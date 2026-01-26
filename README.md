# Pokemon-Game-Corner-Slots

Play now!
[Pokemon Game Corner](https://noah670.github.io/Pokemon-Game-Corner-Slots/).

# 🎰 Pokémon Game Corner Mobile

A mobile-optimized recreation of the classic Pokémon Game Corner from Generation 1-3 (FireRed, LeafGreen, Emerald), featuring slot machines, town exploration, and a prize redemption system.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![React](https://img.shields.io/badge/React-18.x-61dafb.svg)
![Mobile](https://img.shields.io/badge/platform-mobile--first-brightgreen.svg)

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

### Prerequisites
- Node.js 16.x or higher
- npm or yarn package manager

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/pokemon-game-corner.git

# Navigate to project directory
cd pokemon-game-corner

# Install dependencies
npm install

# Start development server
npm run dev
```

The application will open at `http://localhost:5173`

## 🛠️ Technology Stack

- **Frontend Framework**: React 18.x
- **Styling**: Tailwind CSS
- **Icons**: Lucide React
- **Build Tool**: Vite
- **Language**: JavaScript (ES6+)

## 📁 Project Structure

```
pokemon-game-corner/
├── src/
│   ├── components/
│   │   └── PokemonGameCorner.jsx    # Main game component
│   ├── App.jsx                       # App entry point
│   ├── index.css                     # Global styles
│   └── main.jsx                      # React DOM render
├── public/
│   └── assets/                       # Images and sounds (optional)
├── package.json
├── vite.config.js
├── tailwind.config.js
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
Edit the initial state in `PokemonGameCorner.jsx`:

```javascript
const [coins, setCoins] = useState(500); // Change 500 to your desired amount
```

### Modifying Payout Rates
Update the `checkWin` function:

```javascript
if (result[0] === '7') winAmount = bet * 100; // Adjust multipliers here
```

### Adding New Prizes
Extend the `prizeList` array:

```javascript
const prizeList = [
  { name: 'Your Prize', cost: 1000, icon: '🎁' },
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

## 📱 Building for Production

```bash
# Create optimized production build
npm run build

# Preview production build locally
npm run preview
```

Build output will be in the `dist/` directory.

## 🚀 Deployment

### Deploy to Netlify
```bash
npm run build
# Drag and drop the 'dist' folder to Netlify
```

### Deploy to Vercel
```bash
npm run build
vercel --prod
```

### Deploy to GitHub Pages
```bash
npm install gh-pages --save-dev
npm run build
npx gh-pages -d dist
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

- Initial load: ~100KB (gzipped)
- 60 FPS animations
- Mobile-optimized touch events
- Minimal re-renders with React hooks

---

**Made with ❤️ for Pokémon fans everywhere**

⭐ Star this repo if you enjoyed playing!
