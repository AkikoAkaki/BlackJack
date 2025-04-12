# Java Blackjack Game

This is a graphical implementation of the popular card game Blackjack, developed in Java. The game is designed for four players to compete against each other without a dealer. Players aim to achieve the highest card point total without exceeding 21, featuring a sleek GUI built with Java Swing.

## Features

- **Multiplayer Support**: Accommodates four players in a competitive, dealer-less format.
- **Graphical User Interface**: An intuitive and visually appealing GUI powered by Java Swing and AWT.
- **Game Logic**: Implements core Blackjack rules, including hitting, standing, and busting.
- **Card Deck Management**: Utilizes a shuffled 52-card deck with custom card images.
- **Score Calculation**: Dynamically calculates scores, treating Aces as 1 or 11 based on the hand.
- **Win Conditions**: Determines the winner by highest score under 21, with tie-breakers based on card count or shared victory.
- **Custom Dialogs**: Includes interactive dialogs for instructions, bust events, and game-over scenarios.

## Screenshots

<p align="center">
  <img src="https://github.com/user-attachments/assets/aa3f6fca-7e98-4824-8fae-528b6e207ad5" alt="Start Screen" width="400"/>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/df8313ed-8f67-466b-8145-d848c427d7dc" alt="Game Play" width="400"/>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/ea8a5862-6370-499f-a911-19bce716c4b0" alt="Game Over" width="400"/>
</p>


*Note: Screenshots will be added to the `screenshots/` directory once captured.*

## Installation

To set up and run this project locally, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/java-blackjack.git
   ```
   Replace `yourusername` with your GitHub username.
2. **Navigate to the Project Directory**:
  ```bash
  cd java-blackjack
  ```
3. **Compile the Java Files**: Ensure you have Java (JDK 8 or later) installed, then compile the source code:
  ```bash
  javac -d bin src/blackjack/*.java
  ```
4. **Run the Application**: Launch the game from the compiled classes:
  ```bash
  java -cp bin blackjack.BlackJack
  ```

## Usage
- **Start Screen**: Click "Start Game" to begin or "Instructions" to view the rules.
- **Game Play**: Players take turns clicking "Hit" to draw a card or "Stand" to end their turn.
- **Busting**: If a player's score exceeds 21, a bust dialog appears, and they are out of the round.
- **Winning**: The player with the highest score under 21 wins. Ties are resolved by card count; if still tied, players share the victory.
- **Game Over**: A dialog displays the winner and offers options to play again or exit.

## Technologies Used
- **Java**: Core language for game logic and implementation.
- **Java Swing**: Framework for building the graphical user interface.
- **Java AWT**: Used for additional GUI components, event handling, and image rendering.

## Project Structure
```text
java-blackjack/
├── src/
│   └── blackjack/
│       ├── BlackJack.java          # Main entry point
│       ├── BlackJackGUI.java       # GUI setup and game interface
│       ├── Card.java               # Card representation and image handling
│       ├── CustomBustDialog.java   # Dialog for bust events
│       ├── CustomEndGameDialog.java# Dialog for game-over scenarios
│       ├── CustomInstructionsDialog.java # Instructions dialog
│       ├── Deck.java               # Deck management and shuffling
│       ├── GameEventListener.java  # Interface for game event callbacks
│       └── Player.java             # Player state and score calculation
├── images/
│   ├── card_*.png                  # Card images (e.g., card_ace_of_spades.png)
│   └── blackjack_start_screen.png  # Start screen background
├── bin/
│   └── (compiled .class files)     # Compiled output directory
└── README.md                       # This file
```

Note: Ensure the `images/` directory contains all 52 card images and the start screen image.

## License
This project is licensed under the MIT License. See the  file for details.

## Contact
For questions or inquiries, please contact Aki Liu at  `akiliu1116@gmail.com`.
