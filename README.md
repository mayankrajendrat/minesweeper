

#  MineSweeper

##  Table of Contents

1. [Game Explaination](#appexplanation)
2. [Game description](#appdescription)
3. [User Stories](#userstories)
4. [Technologies used](#technologies)
5. [Pseudocode](#pseudocode)
6. [Quick Start](#quickstart)

<a name="appexplanation">

## Game explanation :
The player aims to explore the field without hitting a mine. When it explores a cell with a mine, the game is lost. When it opens a mine-free cell, it learns how many adjacent cells contain a mine. This number is displayed in every cell. From this information, the agent tries to infer which adjacent cells are safe or contain a mine. Known mines are flagged dangerous with a red flag symbol.
</a>

<a name="appdescription">

## Game Description :
Among the width × height cells on the field, n_mines cells contain a mine. The goal of the agent is to identify these mines.

The goal state is to explore all cells that contain no mine, and to flag all cells contain a mine.

On every turn, the player selects a cell and either explores it or flags it as mine. When a cell that contains a mine is explored, the game is lost. When the cell contains no mine, the agent learns how many adjacent cells (0 ≤ N ≤ 8) contain mines. (When N = 0, the adjacent cells are explored immediately.) When a cell is known to contain a mine, it can be flagged as such, as a mental note not to consider it for future exploration. Explored cells are visualized as their number N, or a mine symbol when they contain a mine (in which case the game is lost), and flagged cells are marked by a red flag.

The game is won when all non-mine cells are explored and all mine cells are flagged. The game is lost when the agent explores a mine cell.
</a>

<a name="userstories">

## User Stories

*	As a newbie game player, I want to know the game instruction.
*	As a player, I would like to reset my game any time during the game.
*	As a player, I would like to know the time taken to complete the game.
*	As a player, I want to be able to flag or unflag any cell in the grid.
*	As an  player, I want to be able to customize the game difficulty based on my prefrence.
*	As a player, I want to see how much bomb left for me.
 </a>
 
<a name="technologies">

## Technologies used

This game was written using html, CSS, JavaScript(ES6) and Material Design Bootstrap(UI)
</a>

<a name="pseudocode">

## PSEUDOCODE:

On start the game will generate rows*cols cells and assigned n mines in random places and bind the event for unmasking and flag and update the number of moves and bomb count based on moves using updateFeedback().

### Opening adjacent empty cells

when player clicks a cell, the unmasked class will be add and which will control the display of the cell. Then, the mouse click will be disabled on that clicked cell. The timer will start with the first left click on the grid.

When player clicks empty cell, the surrounded cells - if blank which mean empty cell -will open up until a number or bomb or boundary is reached using recursive function.

Player will win After opening all the cells without clicking on any bomb.
</a>

<a name="quickstart">

## Quick start
- [Download the latest release](https://github.com/mayankrajendrat/minesweeper/archive/master.zip) or 
- Clone the repo `git clone https://github.com/mayankrajendrat/minesweeper.git`
### How to use
Download all the files and open index.html in a modern web browser.
</a>

