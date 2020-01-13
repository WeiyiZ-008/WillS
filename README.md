# Shooting-Robot
Simple version of game Battle City. Simulate by using 2D matrix 
Move the player in four direction and shooting the robot to win the game.

#Project of Data Structure Course
At each turn the player may take one of these actions:
- Stand. In this case, the player does not move or shoot.
- Move one step up, down, left, or right. If the player attempts to move out of the
arena (e.g., down, when on the bottom row), the result is the same as standing. It
is allowable for the player to move to a position currently occupied by a robot. If
no robot occupies that position after the robots have moved, the player survived
the turn.
- Shoot in one of the four directions up, down, left, or right. If there is at least one
robot within 5 steps in that direction (this only matters with anything larger than a
6x6 arena), the nearest one in that direction is the candidate victim. If more than
one robot is nearest (i.e., they occupy the same position), only one robot at that
position is the candidate victim. With 2/3 probability, the candidate victim is
damaged; with 1/3 probability, the shot is ineffective and no robot is damaged. A
robot that has been damaged for the second time is destroyed (i.e., to destroy a
robot takes two shots that hit).

The game allows the user to select the player's action: u/d/l/r for movement,
su/sd/sl/sr for shooting, and just hitting enter for standing. The user may also type q to
prematurely quit the game, or c to have the computer select the player's move.
When it's the robots' turn, each robot picks a random direction (up, down, left, or
right) with equal probability. The robot moves one step in that direction if it can; if the
robot attempts to move out of the arena, however, (e.g., down, when on the bottom
row), it does not move. More than one robot may occupy the same position; in that
case, instead of R, the display will show a digit character indicating the number of
robots at that position (where 9 indicates 9 or more). If after the robots move, a robot
occupies the same position as the player, the player dies.
