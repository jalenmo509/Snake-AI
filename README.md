# Snake-AI

gameLoop(): Starts the game loop by setting a setInterval timer that calls show() repeatedly at a given gameSpeed.
show(): Calls the update() and draw() functions in order, which update and redraw the state of the game.
update(): Clears the canvas, moves the snake, checks for apple collisions, updates the reinforcement learning snake's state, checks for collisions, and sets the appleEaten flag to false.
eatApple(): Checks if the snake's head has collided with an apple, and if so, adds a new tail block and spawns a new apple.
gameOver(): Ends the game and resets the snake's variables. Also updates the high score and epoch number.
checkCollision(): Checks for collisions with walls or the snake's own tail. If a collision is detected, calls gameOver().
draw(): Draws the game's state to the canvas by filling in rectangles for the snake's tail and the apple, and displaying the current score.
createRect(): Helper method that draws a rectangle to the canvas.
Event listeners:
gameSpeedElement: Listens for changes to the game speed input and updates the gameSpeed variable and game loop accordingly.
window: Listens for keydown events and updates the snake's rotation direction based on the pressed arrow key.
RLSnake class: Defines an instance of a reinforcement learning snake with various methods and properties that handle the Q-learning algorithm.
Snake class: Defines an instance of the game's snake with various methods and properties that handle movement and collision detection.
