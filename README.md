# Game-Of-Life
Implemented Game of life with memory optimization

![alt tag](http://i.imgur.com/7uZckVq.gif)


## Memory Savings
Many Implementations of Conway's Game Of Life use require two boards, one for the current step, and one to implement the next step.

In our immplementation, we simply use one board, and two vectors to store the current and previous lines. To do this, we simply retain the current line, and the line above int in a vector. When the current line id finished, then the previous line no linger has any effect on the rest of the board, and therefore is able to be updated. The program them loads the next line into a temp array, continuing the until it reaches the board.


## Credits
Created Ian Granger and Steven Povlitz
