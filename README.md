# Dungeon of Doom  

This is my second Princpiples of Program coursework  where I developed a Java program that allows the human player to explore a dungeon, collect gold, and attempt to escape while avoiding a computer-controlled bot player. 

Check the readme.txt which explains the instruction on how to start.


## Game Protocol Commands:



```bash
1. HELLO
-> Displays the total amount of gold required to win.
-> Example format: Gold to win: <number>
```
```bash
2. GOLD
-> Displays your current gold balance.
-> Example format: Gold owned: <number>
```
```bash
3. PICKUP
-> Picks up the gold on your current location.
Response:
    -> Success: Success. Gold owned: <number>
    -> Fail: Fail. Gold owned: <number>
```
```bash
4. MOVE <direction>
-> Moves your character one square in the indicated direction (N, S, E, or W).
-> Players cannot move into walls.

Response:
-> Success: Success
-> Fail: Fail

```
```bash
5. LOOK
-> Displays a 5x5 grid, showing the map around you.
-> The grid shows walls, empty tiles, gold, exits, and players (P for human, B for bot).
-> You are at the center of the grid.
-> Visible areas outside the map are shown as walls (‘#’).
```
```bash
6. QUIT
-> Quits the game.
-> If you are standing on the exit tile (E) and have enough gold to win, you win the game.

Response:
-> WIN: WIN
-> LOSE: LOSE

```

