In this Tic-Tac-Toe challenge, COMPONENTS, PROPS, and STATE work together to manage the game and user actions. The app has three main parts: Game, Board, and Square.

The Game component keeps track of the game’s history and whose turn it is using STATE. When a player clicks on a square, the handlePlay function updates the STATE, which then updates the board.

The Board component gets the current game STATE as PROPS from Game. It displays the board and handles clicks but does not store any data itself. Each square is a Square component, which gets its value and a function to handle clicks as PROPS from Board. When a player clicks a square, it updates the game’s STATE in Game, which then updates the whole board.

By keeping STATE in Game and passing data down as PROPS, the app stays organized, updates correctly, and is easy to manage.
