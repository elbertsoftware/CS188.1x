Run options:
- Manual play: 
	python pacman.py
	
- Show options: 
	python pacman.py --help

- Run the provided ReflexAgent: 
	python pacman.py -p ReflexAgent

- Run with ReflexAgent for testClassic layout: 
	python pacman.py -p ReflexAgent -l testClassic

- Run with ReflexAgent for mediumClassic layout: 
	python pacman.py --frameTime 0 -p ReflexAgent -k 1 (one ghost)
	python pacman.py --frameTime 0 -p ReflexAgent -k 1 (two ghosts)
	
- Run with MinimaxAgent with different layouts and depth:
	python pacman.py -p MinimaxAgent -l minimaxClassic -a depth=4
	python pacman.py -p MinimaxAgent -l trappedClassic -a depth=3
	python pacman.py -p MinimaxAgent -l mediumClassic -a depth=2

- Run with AlphaBetaAgent with different layouts and depth:	
	python pacman.py -p AlphaBetaAgent -a depth=3 -l smallClassic

- Autograder:
	python autograder.py -q q1 --no-graphics
	python autograder.py -q q2 --no-graphics