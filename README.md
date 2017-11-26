# Tic Tac Toe

The goal of the project is to implement a REST backend for a game of tic-tac-toe.

# Features!

- The client (player) starts a game by making a POST request to /games.
  The POST request contains a representation of a game board, either empty
  (computer starts) or with the first move made (player starts).
  The player/computer can choose either noughts or crosses.

- The backend responds with the location URL of the started game.

- Client GETs the board state from the URL.

- Client PUTs the board state with a new move to the URL.

- Backend validates the move, makes it's own move and updates the game state.
  The updated game state is returned in the PUT response.

- The game is over once the computer or the player gets 3 noughts
  or crosses, horizontally, vertically or diagonally or there are no moves to
  be made.

### Tech

* [KnockoutJS] - standalone JavaScript implementation of the Model-View-ViewModel pattern!
* [Django] - high-level Python Web framework
* [Python] - high-level programming language
* [jQuery] - duh

### Installation

This app requires requires [Python](https://www.python.org/) 3.6 to run.

Git Clone

```sh
$ git clone https://github.com/farhanafayez/TicTacToe
```

Install the dependencies from requirements.txt by creating and activating a new virtual environment however you wish. Ex: Conda etc.

```sh
$ cd src/tictactoe/
$ pip install requirements.txt
```

### Running the application

```sh
$ cd src/tictactoe/
$ python manage.py runserver
$ Open browser http://127.0.0.1:8000/game
```




