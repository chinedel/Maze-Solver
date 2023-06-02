MAZE SOLVER “MVP SPECIFICATION”
This is a maze solver that can load your maze from a binary file and show its solution in the web browser.
Take a glimpse at the expected structure of the project. Once finished, the project will look as follows:

    
This maze is enclosed in a rectangle comprising a grid of square cells that form passages along straight lines. Solving the maze means finding a path leading from the entrance to the exit.

Most squares won’t have any role in the maze. However, at least two of them must be marked as the entrance and the exit, respectively. They will tell the pathfinding algorithm where to start and finish its journey. Some other squares can be marked as obstacles like walls, enemies, or the exterior, which you can’t cross. Finally, a few squares can contain rewards, like bonus points or power-ups that may influence the path.



All in all, there are six unique roles.
1.	Enemy
2.	Entrance
3.	Exit
4.	Exterior
5.	Reward
6.	Wall
# models/role.py

from enum import IntEnum, auto

class Role(IntEnum):
    ENEMY = auto()
    ENTRANCE = auto()
    EXIT = auto()
    EXTERIOR = auto()
    REWARD = auto()
    WALL = auto()

