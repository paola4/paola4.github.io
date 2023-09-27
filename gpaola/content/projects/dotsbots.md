---
title: "Dots and Bots"
image: /images/projects/DotsBots/play.png
showonlyimage: true
Description: A terminal-based implementation of the traditional Dots and Boxes game in Python using Mini Max algorithm with Alpha-Beta pruning.
tags:
- AI
- Python
- Game Development
- Min-Max
---
## About the Project
This is a terminal-based version of the classic 'Dots and Boxes' game, a zero-sum game for two players that is easily played with pencil and paper. The game begins with a grid of dots, and players take turns connecting two dots with a single line. If a player successfully completes the fourth side of a box, the player gets another turn. The player continues to play another turn as long as they complete a box. Otherwise, the turn switches to their opponent. The game ends when there are no more dots left to connect; the winner is the player with the most points (1 point earned per box that is completed).

## Technical Details
The Dots and Boxes program includes four files:

* board.py
* box.py
* dotsAndBoxes.py
* miniMax.py

This is a terminal-based game, created using Python. To play, the user should input: `python3 dotsAndBoxes.py 3 3` (or whatever the preferred board size is) into their terminal. The program works with grids of all sizes, although larger grids result in increasingly slower 'moves' by the AI as it attempts to search larger game trees. The AI is implemented using the <a href="https://en.wikipedia.org/wiki/Minimax">mini-max recursive algorithm</a> with Alpha-Beta pruning. 

## Interface Screenshots
#### Sample Initial Menu:

The user can select from three game-play options: Player vs. AI, Player vs. Player, and AI vs. AI.

<figure class="image is-569x160">
<img src="/images/projects/DotsBots/main1.png">
</figure>


For games played against the AI, the player may additionally select the game's difficulty (the depth to which the game will search the game tree for the AI's next-move) and whether they want to play first or second:

<figure class="image is-569x160">
<img src="/images/projects/DotsBots/main2.png">
</figure>

  
#### In-Game Interface:
The in-game interface allows for the user to access a help-menu with the several options. The player enters their move as two tuples, each representing a coordinate for the dots they want to connect with a line.
<figure class="image is-569x315">
<img src="/images/projects/DotsBots/main3.png">
</figure>