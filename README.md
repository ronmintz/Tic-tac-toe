# Tic-tac-toe
Tic-tac-toe game.  To run, do in this directory:

npm install -g http-server

http-server -c-1

localhost:8080

Click on standalone.html

This puts up the tic-tac-toe board.  Alternately, click on square where you want to enter X.  Then click on square where you want to enter O.  Repeatedly, enter X's and O's alternately until "Winner is X or O" appears or all squares are filled.

Possible further improvements:
1. Don't respond to clicking on a square that is filled.  This is implemented by returning from the function passed to onClick with no action if the filled state of the square is true.

2. When there is a winner, don't respond to any further clicks.  This is implemented by setting a winnerExists state in Board when checkForWinner(gameState) returns true.  Pass this state to Square and return from the function passed to onClick with no action if winnerExists == true.

