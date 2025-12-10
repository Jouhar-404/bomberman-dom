# 💣 Bomberman DOM

A real-time multiplayer Bomberman game built with vanilla JavaScript, DOM manipulation, and WebSockets. No canvas, no WebGL - just pure DOM performance optimization!

## 🎮 Game Overview

Battle against 2-4 players in this classic Bomberman-style arena! Place bombs strategically, collect power-ups, and be the last player standing. Built using a custom DOM framework with WebSocket synchronization for smooth multiplayer gameplay.

## ✨ Features

### Core Gameplay
- **Multiplayer Support**: 2-4 players in real-time battles
- **Three Lives System**: Each player starts with 3 lives
- **Dynamic Map Generation**: Randomly generated destructible blocks with fixed wall patterns
- **Power-Up System**:
  - 💣 **Bombs**: Increase simultaneous bomb capacity
  - 🔥 **Flames**: Extend explosion range
  - ⚡ **Speed**: Boost movement speed

### Technical Highlights
- **60+ FPS Performance**: Optimized using `requestAnimationFrame`
- **Zero Frame Drops**: Efficient DOM manipulation
- **WebSocket Chat**: Real-time player communication
- **Custom Framework**: Built on top of mini-framework project
- **Smart Matchmaking**: 
  - Game starts with 2+ players after 20 seconds
  - Instant start with 4 players
  - 10-second countdown before game begins

## 🚀 Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn
- Modern web browser (Chrome, Firefox recommended)

### Installation

1. **Clone the repository**
```bash
git clone <your-repo-url>
cd bomberman-dom
```

2. **Install dependencies**
```bash
npm install
```

3. **Start the server**
```bash
npm start
```

4. **Open the game**
```
Navigate to http://localhost:3000 in your browser
```

### Running Multiple Players

To test multiplayer functionality:
1. Open the game URL in multiple browser windows/tabs
2. Enter a different nickname for each player
3. Wait for players to join or start with 2+ players

## 🎯 How to Play

### Controls
- **Arrow Keys** or **WASD**: Move your character
- **Space**: Place a bomb

### Game Rules
1. **Starting Position**: Players spawn in the four corners of the map
2. **Lives**: Each player has 3 lives - lose all lives and you're out
3. **Objective**: Be the last player standing
4. **Bombs**: Explode after a few seconds, destroying blocks and players in range
5. **Power-ups**: Appear randomly when blocks are destroyed

### Winning Strategy
- Trap opponents with strategic bomb placement
- Collect power-ups to become stronger
- Use destructible blocks as temporary cover
- Manage your bomb count wisely

## 🗂️ Project Structure

```
bomberman-dom/
├── src/
│   ├── framework/       # Custom DOM framework
│   ├── game/           # Game logic
│   │   ├── player.js
│   │   ├── bomb.js
│   │   ├── map.js
│   │   └── powerups.js
│   ├── multiplayer/    # WebSocket handling
│   │   ├── socket.js
│   │   └── chat.js
│   └── utils/          # Performance utilities
├── public/
│   ├── index.html
│   ├── styles/
│   └── assets/
├── server/             # WebSocket server
└── package.json
```

## 🔧 Technical Implementation

### Performance Optimization
- **RequestAnimationFrame Loop**: Smooth 60fps gameplay
- **Delta Time Calculations**: Frame-independent movement
- **Efficient DOM Updates**: Minimal reflows and repaints
- **Performance Monitoring**: Built-in FPS counter

### WebSocket Architecture
- Real-time game state synchronization
- In-game chat system
- Player connection/disconnection handling
- Lobby system with automatic matchmaking

### Framework Usage
Built entirely with the custom mini-framework, demonstrating:
- Component-based architecture
- Event handling system
- State management
- DOM manipulation without virtual DOM

---

**Made with 💣 and ⚡ | 60fps guaranteed**
