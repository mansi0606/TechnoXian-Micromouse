For TechnoXian 2024 I have been a part of autonomy team representing IIT Indore. We had come up with final two algorithms, Flood Fill and A* Algorithm.
Flood Fill Algorithm for Micromouse on Arduino:
Here’s a concise and practical approach for implementing the Flood Fill algorithm on an Arduino-based micromouse. The code in the file "Arduino Code" assumes a square maze (typically 16x16), represented as a 2D array, and updates cell distances as new walls are discovered.

Key Components
Maze Representation: Each cell stores its wall configuration and distance.

Flood Fill Logic: After every movement and wall update, the algorithm recalculates cell distances.

Movement Decision: The micromouse selects the neighbor with the lowest flood value not blocked by a wall.
Sensor Integration: Call updateCellWalls() after each move, passing sensor results to update wall information.

Flood Fill Update: Always call updateFloodFill() after discovering a new wall.

Modularity: Abstract motor and sensor functions so you can focus on maze logic and test with simulators.

References
For further example sketches and full Arduino projects with floodfill logic, see public repositories and discussions.

Implementations may involve additional features such as wall memory arrays, direction enums, and hardware abstraction for optimizing turning and movement.

This framework is adaptable; you may optimize memory or adjust the maze size and wall-handling code to fit your specific setup.
The A* algorithm is a pathfinding technique that finds the shortest route between two points using a combination of actual travel cost and a heuristic estimate to the goal. 
It efficiently explores possible paths, always choosing the option that appears most promising based on both cost so far and estimated cost remaining.
