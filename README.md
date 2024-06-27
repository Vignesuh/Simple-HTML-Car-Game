# Simple-HTML-Car-Game Korangle Softwares internship Problem
#SOLVED
## Description
This is a simple car game where you control a car using arrow keys to avoid enemy cars. The speed of the car increases every 5 seconds and you earn points by passing enemy cars.

## Features
- Start the game by clicking the start screen.
- Control the car using arrow keys.
- Avoid collision with enemy cars.
- Speed increases every 5 seconds starting from 5.
- Earn 10 points for each enemy car you pass.

## How to Play
1. Click on the start screen to begin the game.
2. Use arrow keys to move your car:
   - Up Arrow: Move up
   - Down Arrow: Move down
   - Left Arrow: Move left
   - Right Arrow: Move right
3. Avoid colliding with enemy cars.
4. Earn points by passing enemy cars.
5. The game ends if you collide with an enemy car.

## Updates and Changes

### 1. Increase Speed
- The player's speed starts at 5 and increases by 1 every 5 seconds.
- The speed is reset to 5 whenever the game restarts.
- Added a timer that increments the player's speed every 5 seconds using `setInterval`.

### 2. Score Increment Logic
- The score is incremented by 10 only when the rear end of `myCar` has passed the rear end of an `enemyCar`.
- Modified the `moveEnemy` function to check if `myCar` has passed the `enemyCar` before incrementing the score.
- Used an array `passedCars` to keep track of enemy cars that have been passed to avoid multiple scoring for the same car.

### Common Mistakes Avoided
1. Starting speed is always 5 after restarting the game.
2. Speed increments correctly every 5 seconds without speeding up after multiple restarts.
3. Score increments only when `myCar` passes `enemyCar`, not when enemy cars pass the end of the screen.
4. Ensured the score increments properly even if `myCar` is moving upwards at the time of passing.
5. Score does not increment continuously as before.

## How to Install
1. Clone the repository or download the `car.html` file.
2. Place the file in a directory and open it in a web browser.

## How to Run
- Open the `car.html` file in any modern web browser.
- Click on the start screen to begin playing.

## Files
- `car.html`: The main HTML file containing the game code and logic.
