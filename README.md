# Chess Engine built using NegaMax algorithm and Alpha-Beta Pruning

This project is a simple chess engine implemented using the Negamax algorithm with alpha-beta pruning. The engine evaluates possible moves and selects the best move to play. The game can be played against the AI or another player. Testing the thought processes of the AI can be done by pairing the AI against itself.

## Features

- Uses the NegaMax algorithm (a variant of the Minimax algorithm) by building a game tree and recursively traverses the tree with the assumption that the opponents moves are simply the negations of the player's moves.
- Uses the Alpha-Beta Pruning optimization technique to reduce the number of nodes evaluated in the game search tree and hence improve efficiency.
- Implements a simple GUI using PyGame to allow for visual representations of moves.

## Installation

To install the necessary dependencies, you can use pip:

```bash
pip install -r requirements.txt

```

## Usage

In order to use this project, first ensure that the player settings in the main.py file are set accordingly. Player one represents white and Player two represents black. To play as the intended color, set the respective variable to True (the one that is set to false will be played by the AI) in the main.py file. If both are set to True, then the game will behave as a 2 player game. The AI can also be paired against it by setting both to False. The depth of the game search tree can be controlled by modifying the set_depth variable in the ai.py file. The higher the set_depth value, the better the AI will play. However, the game is more likely to crash if the value is very high. For performance and optimum results, set the depth to 4.

To run the file, run the following command in a terminal,

```bash
python main.py

```

## License

This project is licensed under the Creative Commons Zero license. See the LICENSE file for more details.
