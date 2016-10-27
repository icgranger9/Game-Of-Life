# Game-Of-Life

![alt tag](http://i.imgur.com/7uZckVq.gif)


## Memory Savings
Most Implementations of Conway's Game Of Life usually require two boards. One for the current step, and one to store the next step.

In our immplementation, we simply use one board and two vectors to store the current and previous lines. To achieve this efficiency, we simply retain the current line and the line above it in a vector. When the current line is finished, then the previous line no longer has any effect on the rest of the board, and therefore is able to be saved. The program them loads the next line into a temp array, continuing  until it reaches the end of the board.


## Credits
Created Ian Granger and Steven Povlitz
