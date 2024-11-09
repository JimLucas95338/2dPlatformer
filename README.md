# 🎮 2D Platform Game

<div align="center">

![Game Preview](preview.gif)

A modern, responsive platformer game built with vanilla JavaScript and HTML5 Canvas.

[Play Demo](https://JimLucas95338.github.io/2dPlatformer) | [Report Bug](https://github.com/JimLucas95338/2dPlatformer/issues) | [Request Feature](https://github.com/JimLucas95338/2dPlatformer/issues)

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]

</div>

## 📋 Table of Contents
- [About The Project](#about-the-project)
  - [Built With](#built-with)
  - [Key Features](#key-features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [How to Play](#how-to-play)
- [Game Architecture](#game-architecture)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)
- [Acknowledgments](#acknowledgments)

## 🎯 About The Project

### What Makes This Game Special
This 2D platformer game showcases fundamental game development concepts while providing an engaging gaming experience. Built with a focus on:

- Clean, maintainable code architecture
- Smooth, physics-based movement
- Precise collision detection
- Responsive controls
- Expandable game engine design

### Built With
- 🎨 HTML5 Canvas for rendering
- 💻 Vanilla JavaScript for game logic
- 🎭 CSS for styling
- 📱 Responsive design principles

### Key Features
Current implementation includes:
- ⚡ Smooth player movement with acceleration and friction
- 🎮 Precise platform collisions from all directions
- 🌟 Physics-based jumping mechanics
- 🎨 Multiple platforms at different heights
- 🔄 Efficient game loop
- 📱 Cross-browser compatibility

## 🚀 Getting Started

### Prerequisites
- Any modern web browser (Chrome, Firefox, Safari, Edge)
- Basic understanding of HTML/JavaScript (for development)
- Local development server (optional)

### Installation

1. **Clone the Repository**
```bash
git clone https://github.com/JimLucas95338/2dPlatformer.git
```

2. **Navigate to Project Directory**
```bash
cd 2dPlatformer
```

3. **Launch the Game**
- Option 1: Open `index.html` directly in a browser
- Option 2: Use a local development server
```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx serve
```

## 🎮 How to Play

### Controls
| Key | Action |
|-----|--------|
| ← | Move Left |
| → | Move Right |
| ↑ | Jump |

### Game Mechanics
- Use arrow keys to move left and right
- Jump between platforms with the up arrow
- Movement features acceleration and friction for smooth control
- Collide with platforms from all sides
- Fall off a platform and you'll return to the start

## 🏗 Game Architecture

### Core Components

#### Physics System
```javascript
// Physics properties
const physics = {
    gravity: 0.5,
    friction: 0.8,
    jumpForce: 12
};

// Movement update example
player.velocityY += gravity;
player.y += player.velocityY;
player.velocityX *= friction;
```

#### Collision System
```javascript
// Collision detection with platforms
function checkCollision(player, platform) {
    return player.x < platform.x + platform.width &&
           player.x + player.width > platform.x &&
           player.y < platform.y + platform.height &&
           player.y + player.height > platform.y;
}
```

### Project Structure
```
2dPlatformer/
│
├── index.html            # Main game file
│   ├── Player Logic     # Player movement and physics
│   ├── Platform Logic   # Platform creation and collision
│   └── Game Loop       # Main update and render cycle
│
├── README.md            # Documentation
└── LICENSE             # MIT license
```

## 📌 Roadmap

### Phase 1 - Core Mechanics ✓
- [x] Basic player movement
- [x] Jumping physics
- [x] Ground collision
- [x] Platform collision
- [x] Smooth movement with acceleration
- [x] Multiple platforms

### Phase 2 - Enhanced Gameplay
- [ ] Moving platforms
- [ ] Double jump ability
- [ ] Wall sliding/jumping
- [ ] Sprint ability
- [ ] Variable jump heights

### Phase 3 - Content
- [ ] Multiple levels
- [ ] Collectibles
- [ ] Enemies
- [ ] Power-ups
- [ ] Score system

### Phase 4 - Polish
- [ ] Character sprites
- [ ] Animation system
- [ ] Sound effects
- [ ] Background music
- [ ] Particle effects
- [ ] Screen transitions

## 🤝 Contributing

We welcome contributions! Here's how you can help:

1. **Fork** the Project
2. **Create** your Feature Branch
   ```bash
   git checkout -b feature/AmazingFeature
   ```
3. **Commit** your Changes
   ```bash
   git commit -m 'Add some AmazingFeature'
   ```
4. **Push** to the Branch
   ```bash
   git push origin feature/AmazingFeature
   ```
5. Open a **Pull Request**

### Contribution Guidelines
- Write clean, commented code
- Follow existing code style
- Update documentation as needed
- Test thoroughly before submitting

## 📝 License

Distributed under the MIT License. See `LICENSE` for more information.

## 📫 Contact

Jim Lucas - [@JimLucas95338](https://github.com/JimLucas95338)

Project Link: [https://github.com/JimLucas95338/2dPlatformer](https://github.com/JimLucas95338/2dPlatformer)

## 👏 Acknowledgments

* [HTML5 Game Devs Forum](https://html5gamedevs.com/)
* [MDN Web Docs](https://developer.mozilla.org/)
* [Game Programming Patterns](https://gameprogrammingpatterns.com/)

---

<div align="center">
Made with ❤️ by Jim Lucas

Don't forget to give the project a star ⭐ if you like it!
</div>

<!-- MARKDOWN LINKS & IMAGES -->
[contributors-shield]: https://img.shields.io/github/contributors/JimLucas95338/2dPlatformer.svg?style=for-the-badge
[contributors-url]: https://github.com/JimLucas95338/2dPlatformer/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/JimLucas95338/2dPlatformer.svg?style=for-the-badge
[forks-url]: https://github.com/JimLucas95338/2dPlatformer/network/members
[stars-shield]: https://img.shields.io/github/stars/JimLucas95338/2dPlatformer.svg?style=for-the-badge
[stars-url]: https://github.com/JimLucas95338/2dPlatformer/stargazers
[issues-shield]: https://img.shields.io/github/issues/JimLucas95338/2dPlatformer.svg?style=for-the-badge
[issues-url]: https://github.com/JimLucas95338/2dPlatformer/issues
[license-shield]: https://img.shields.io/github/license/JimLucas95338/2dPlatformer.svg?style=for-the-badge
[license-url]: https://github.com/JimLucas95338/2dPlatformer/blob/master/LICENSE
