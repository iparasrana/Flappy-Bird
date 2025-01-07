# Flappy Bird Game

This project implements a simple version of the Flappy Bird game using Java's built-in AWT and Swing libraries. The game involves controlling a bird to pass through pipes without colliding. Below are the details of the implementation and instructions to run the game.

## Features

- **Game Loop**: The game runs on a timer-based game loop that updates the game state and renders the graphics.
- **Graphics**: Uses AWT and Swing to draw the background, bird, pipes, and score.
- **Dynamic Pipes**: Pipes are randomly generated at intervals and move across the screen.
- **Collision Detection**: Detects collisions between the bird and pipes, or when the bird goes out of bounds.
- **Score Tracking**: Displays the current score on the screen, which increases as the bird successfully passes pipes.
- **Restart Mechanism**: Allows restarting the game by pressing the space bar after a game over.

## Classes and Components

### Main Class: `FlappyBird`

- Extends `JPanel` and implements `ActionListener` and `KeyListener`.
- Manages the game state, rendering, and input handling.

### Bird
- Represents the bird controlled by the player.
- Includes properties such as position, size, and image.

### Pipe
- Represents a pipe (either top or bottom) in the game.
- Includes properties such as position, size, image, and whether it has been passed by the bird.

## Key Variables

- **Board Dimensions**: `boardWidth` and `boardHeight` define the size of the game window.
- **Bird Movement**: `velocityY` and `gravity` control the bird's vertical movement.
- **Pipe Movement**: `velocityX` controls the speed at which pipes move left.
- **Score**: Tracks the player's progress by counting passed pipes.

## How to Run

1. **Prerequisites**:
   - Ensure you have Java installed on your system.
   - Add the required images to the project directory:
     - `flappybirdbg.png` (background image)
     - `flappybird.png` (bird image)
     - `toppipe.png` (top pipe image)
     - `bottompipe.png` (bottom pipe image)

2. **Compile**:
   - Compile the program using the `javac` command:
     ```bash
     javac FlappyBird.java
     ```

3. **Run**:
   - Execute the program using the `java` command:
     ```bash
     java FlappyBird
     ```

4. **Gameplay**:
   - Press the space bar to make the bird jump.
   - Avoid colliding with pipes or going out of bounds.
   - The game restarts automatically after a game over when the space bar is pressed.

## Notes

- Make sure the image files are in the same directory as the `.java` file, or adjust the paths in the code.
- The game speed and difficulty can be adjusted by modifying `velocityX`, `gravity`, or the `placePipeTimer` interval.

## Future Enhancements

- Add sound effects for jumps and collisions.
- Introduce multiple levels with increasing difficulty.
- Implement a high-score tracking feature.
- Enhance graphics with animations or additional assets.

Enjoy playing Flappy Bird!

