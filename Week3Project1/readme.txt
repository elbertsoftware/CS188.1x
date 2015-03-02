Run options:
- Manual play: 
	python pacman.py
	
- Show options: 
	python pacman.py --help

- Use GoWestAgent on testMaze: 
	python pacman.py --layout testMaze --pacman GoWestAgent

- Use GoWestAgent on tinyMaze:
	python pacman.py --layout tinyMaze --pacman GoWestAgent
	
- Use tinyMazeSearch agent on tinyMaze (hard coded path for tinyMaze only)
	python pacman.py -l tinyMaze -p SearchAgent -a fn=tinyMazeSearch
	
- Test DFS implementation (Stack):
	python pacman.py -l tinyMaze -p SearchAgent -a fn=dfs
	python pacman.py -l mediumMaze -p SearchAgent -a fn=bfs
	python pacman.py -l bigMaze -p SearchAgent -a fn=bfs -z .5 --frameTime 0
	
- Test BFS implementation (Queue):
	python pacman.py -l tinyMaze -p SearchAgent -a fn=bfs
	python pacman.py -l mediumMaze -p SearchAgent -a fn=bfs
	python pacman.py -l bigMaze -p SearchAgent -a fn=bfs -z .5 --frameTime 0
	
- Test USC implementation (PriorityQueue):
	python pacman.py -l tinyMaze -p SearchAgent -a fn=usc
	python pacman.py -l mediumMaze -p SearchAgent -a fn=usc
	python pacman.py -l bigMaze -p SearchAgent -a fn=usc -z .5 --frameTime 0
	
	python pacman.py -l mediumDottedMaze -p StayEastSearchAgent (cost: StayEast: 646; USC: 68)
	python pacman.py -l mediumScaryMaze -p StayWestSearchAgent (cost: StayWest: 418; USC: less but lost)
	
	python pacman.py -l openMaze -p SearchAgent -a fn=ucs -z .5
	
- Test USC implementation (PriorityQueueWithFunction):
	python pacman.py -l bigMaze -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic -z .5
	python pacman.py -l openMaze -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic -z .5
	
- Test BFS with CornersProblem
	python pacman.py -l tinyCorners -p SearchAgent -a fn=bfs,prob=CornersProblem
	
- Autograder:
	python autograder.py
	python autograder.py -q q?