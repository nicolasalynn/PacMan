# Solving PacMan with Search Algorithms

This project demonstrates some generic implementations of uninformed and informed search algorithms by solving PacMan puzzles.
Specifically, Depth First Search (DFS), Breadth First Search (BFS), Uniform Cost Search (UCS), and A* are implemented. 

The implementations shown here are developed as as a solution to the AI Nanodegree Udacity program which uses UC Berkley's PacMan Search project
found here: http://ai.berkeley.edu/search.html. 

**Relevant Code** 
1. seach.py
2. searchAgent.py
3. util.py

**Demonstrations**
1. DFS: ``` python pacman.py -l bigMaze -z .5 -p SearchAgent --frameTime 0 ```
2. BFS: ``` python pacman.py -l bigMaze -p SearchAgent -a fn=bfs -z .5 --frameTime 0```
3. A* : ``` python pacman.py -l bigMaze -z .5 -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic --frameTime 0```
4. Finding Corners: ```python pacman.py -l mediumCorners -p SearchAgent -a fn=bfs,prob=CornersProblem --frameTiem 0```
5: Finding Corners (with heuristic): ```python pacman.py -l mediumCorners -p AStarCornersAgent -z 0.5```
6. Eating All Dots: ```python pacman.py -l mediumCorners -p AStarCornersAgent -z 0.5 --frameTime 0```
7. Eating All Dots (with heuristic): ```python pacman.py -l mediumCorners -p AStarCornersAgent -z 0.5 --frameTime 0```

**Notes**

The heuristic strategy implemented works by taking a given coordinate or current state and finding a route that minimizes the manhattan distance of the susequent path. 
The heuristic is implemented by adding an additional cost to a particular node on the frontier of the A* search algorithm. 

