# Title: Enhancing Pacman's Navigation: A Journey through Search Algorithms and Heuristics

## Introduction:
In this project, we embarked on a thrilling adventure to implement various search algorithms and intelligent heuristics for our beloved Pacman. Our goal was to optimize Pacman's ability to navigate a complex maze, locate food pellets efficiently, and ultimately triumph over the challenges that lay ahead. By experimenting with depth-first search, breadth-first search, A*, and uniform cost search (UCS), we sought to uncover the strengths and weaknesses of each approach and design a Pacman agent capable of making intelligent decisions.

## The Quest Begins - Search Algorithms(Breadth-First-Search and Depth-First-Search)
Our first step in empowering Pacman was to equip it with search algorithms. We implemented depth-first search, which boldly delves into the deepest nodes in the frontier, and breadth-first search, which steadfastly explores all nodes at the current depth level before venturing deeper. While depth-first search proved to be less costly in certain situations, breadth-first search exhibited optimality by finding the most efficient path.

## The Power of Heuristics - A* and UCS
The allure of intelligent heuristics led us to incorporate A* and UCS into Pacman's arsenal. A* search emerged as the shining star by combining the best of UCS and greedy best-first search. Utilizing a heuristic function, namely the Manhattan distance, A* efficiently estimated the cost from each node to the goal, resulting in faster search times and fewer node expansions compared to other algorithms. Meanwhile, UCS provided a foundation for further exploring the maze and solidifying Pacman's knowledge of the terrain.

## Uncovering the Corners - Detecting Food Pellets
Pacman's ultimate test lay in locating food pellets scattered throughout the maze. We rose to the challenge and successfully detected the four food pellets residing in the maze's corners. This crucial information allowed Pacman to plan its route and devise strategies for a victorious pursuit of nourishment.

##  The Enigma of the Corner Problem - Heuristic Solution
An enigmatic puzzle presented itself: Which corner should Pacman visit last? With determination, we devised a heuristic solution to address this corner problem. By assigning the longest Manhattan distance as the heuristic value for the corner to be visited last, we prioritized its exploration. We continuously recalibrated the heuristic based on the closest unvisited corner, effectively guiding Pacman through the corners' intricate maze.

## Devouring All the Dots - Efficient Food Collection
With knowledge of food pellet locations in hand, we tackled the challenge of collecting them optimally. A list of all food positions in the maze enabled us to calculate each node's heuristic value, representing Pacman's distance to the nearest food pellet. Leveraging this information, we discerned the farthest food pellet from Pacman, propelling it toward the most distant reward.

## Suboptimal Search - Finding the Nearest Food Pellet
Equipped with a breadth-first search algorithm, we crafted a suboptimal search strategy to uncover the food pellet closest to Pacman. This implementation harnessed the isGoalState function to determine whether food pellets existed at specific positions, steering Pacman toward its nearby sustenance.

## Conclusion:

Our Pacman project was an enthralling journey filled with challenges, triumphs, and groundbreaking discoveries. By harnessing the power of diverse search algorithms and astute heuristics, we elevated Pacman's navigation capabilities to new heights. From efficiently collecting food pellets to deftly maneuvering through corners, our Pacman agent now stands as a symbol of intelligent design and strategic thinking. As we conclude this remarkable quest, we look forward to future endeavors where we can continue to explore and refine the world of artificial intelligence and game agent development.
