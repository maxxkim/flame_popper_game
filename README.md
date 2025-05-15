Flame Bubble Pop
A fun and interactive bubble popping game built with Flutter and the Flame game engine.
Show Image
📖 Description
Flame Bubble Pop is a simple yet addictive game where players pop colorful bubbles that appear on the screen. The game features:

Randomly spawning bubbles with different sizes
Score tracking based on bubble size (smaller bubbles = higher points)
Gradually increasing difficulty as bubbles spawn faster
Various background options (solid color, gradient, or image)
Animated bubble popping effects with particles
SVG-based graphics (when available)

🚀 Getting Started
Prerequisites

Flutter SDK (latest stable version recommended)
Dart SDK
An IDE (VS Code, Android Studio, etc.)

Installation

Clone this repository:
bashgit clone https://github.com/yourusername/flame-bubble-pop.git
cd flame-bubble-pop

Install dependencies:
bashflutter pub get

Run the application:
bashflutter run


🎮 How to Play

Tap/click on bubbles to pop them
Earn more points by popping smaller bubbles
Bubbles will disappear after a few seconds if not popped
The game speeds up over time, with bubbles spawning more frequently

🧩 Project Structure
lib/
├── background/
│   ├── background.dart         # Solid color background
│   ├── gradient_background.dart # Gradient background
│   ├── image_background.dart   # Image background
├── bubble.dart                 # Bubble component implementation
├── bubble_game.dart            # Main game logic
└── main.dart                   # Entry point
🔧 Customization
The game can be customized in several ways:
Backgrounds
You can choose from three background types:

BackgroundType.solid - A solid color background
BackgroundType.gradient - A gradient background
BackgroundType.image - An image background

dart// Example of customizing the game
final game = BubbleGame(
  backgroundType: BackgroundType.gradient,
  bgColor: Colors.purple, // For solid background
  gradientColors: [Colors.purple, Colors.blue], // For gradient background
  backgroundImagePath: 'assets/images/custom_background.png', // For image background
);
Assets
The game looks for the following assets:

pop.png - Popping animation sprite
bubble.png - Optional bubble sprite (falls back to a circle if not found)
background.png - Default background image
images/musician.svg and images/forecaster.svg - Optional SVG content for bubbles
images/pop.svg - Optional SVG pop animation

Make sure to add your assets to the pubspec.yaml file:
yamlflutter:
  assets:
    - assets/images/pop.png
    - assets/images/bubble.png
    - assets/images/background.png
    - assets/images/musician.svg
    - assets/images/forecaster.svg
    - assets/images/pop.svg
🧪 Testing
Run the tests using:
bashflutter test
📚 Dependencies

Flame - Game engine for Flutter
flame_svg - SVG support for Flame

🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

Fork the repository
Create your feature branch (git checkout -b feature/amazing-feature)
Commit your changes (git commit -m 'Add some amazing feature')
Push to the branch (git push origin feature/amazing-feature)
Open a Pull Request

📝 License
This project is licensed under the MIT License - see the LICENSE file for details.
👏 Acknowledgements

Flame Engine - For the amazing game engine
Flutter - For the UI toolkit


Made with ❤️ using Flutter and Flame
