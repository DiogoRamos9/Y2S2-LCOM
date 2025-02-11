# LCOM

In this repository there is available every LCOM lab solved and the final project of the course (grade: 17/20) that will be the focus of this README.

# SpaceCOM Shooter

This project was developed for the **Laboratório de Computadores** (Computer Laboratory) 2023-2024 course at **FEUP** on the **MINIX** Operating System. It is a original space shooter game, which the goal is to destroy the maximum number of incoming asteroids and try to not collide with them. The game has a variety of features to make it more difficult, like the speed of asteroids incresing during the game, more fun, like power that be activated to help the player, etc. For more details checkout out our [official report](proj/doc/lcom_proj.pdf).

![menu_start_selected](https://github.com/user-attachments/assets/6c7543cc-9eaf-44c1-8867-99e74a14772c)


## Architecture

The architecture of the project is modular, with each module handling a specific aspect of the game, using the **MVC** model. The main components are:

- **Game Logic**: Managed in the `game/` directory, this includes the main game loop, state transitions, and game mechanics.
- **Game States**: Each game state (e.g., menu, game, settings) is managed by its own controller in the `game/gameStates/` directory.
- **Sprites**: Managed in the `sprites/` directory, this includes loading, drawing, and animating sprites.
- **Utilities**: General utility functions and hardware interaction code are located in the `utils/` directory. This includes keyboard and mouse input, real-time clock (RTC), timer, and video functions. These are the functions that were developed throughout the whole semester during classes.
- **Images**: All XPM image files used in the game are stored in the `imgs/` directory.

## Features

- **Multiple Game States**: The game includes various states such as menu, game, settings, instructions, game over, leaderboard, and pause.
- **Sprite Management**: Efficient loading, drawing, and animating of sprites.
- **Real-Time Clock Display**: Toggle the display of the real-time clock in the menu.
- **Keyboard and Mouse Input**: Responsive controls for navigating menus and playing the game.
- **High Scores**: Functional to display high scores.
- **Pause Functionality**: Ability to pause the game and resume later.
- **Settings Menu**: Customize game settings to enhance the gaming experience.
- **Game Logic**: The whole game logic and mechanisms using the hardware interaction, including collision detection, firing lasers upon mouse click, change cannon's direction, etc.
- **Dynamic Difficulty**: As the player increases his score, the Difficulty Controller makes the game harder, with more asteroids spawning and them getting faster.
- **Powerups**: To make the game more fun, we added power-ups for the player to catch with the mouse during the game. There are two powerups: the bomb, when the player clicks on the bomb, every asteroid on the screen is exploded, and the coin, that adds 5 to the current score.
- **Instructions Menu**: There is an intuitive menu for instructions on how to play the game.

## Prints of the Game

### Gameplay:

![game](https://github.com/user-attachments/assets/9e15c0b0-96f1-4689-9c57-21ac073d9edc)



### Pause:

![pause](https://github.com/user-attachments/assets/f25c9e92-ed6d-4584-9402-c9c464acd292)




### Instructions Menu:

![instruct](https://github.com/user-attachments/assets/f1f59b1b-a8ce-425b-a0d9-1f1e47ac29fb)



### Settings Menu:

![set](https://github.com/user-attachments/assets/039c138f-4794-4c31-b86c-c5903f70ec52)



## Authors

- Diogo Ramos (up202207954)
- Gabriel Braga (up202207784)
- Guilherme Rego (up202207041)
