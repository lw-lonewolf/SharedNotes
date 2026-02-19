#sixth_semester
# Problem Solving Agent 
* Steps
	* Goal Formulation
	* Problem Formulation
	* Search
	* Execute
## Goal Formulation
The process of defining what an agent aims to achieve based on its current state and the criteria used to measure success. It enables the agent to focus on a specific objective and determine the most appropriate sequence of actions required to achieve that goal.

>[!example] Example
>* An agent is currently at A in a map. Its task is to reach location B with the shortest possible distance 
> **Current State:** Agent is at A
> **Goal:** Agent must reach B
> **Success Measure:** Minimum distance or minimum time
> **Result of goal formulation:** Agent decides to find the shortest path from A to B using an appropriate strategy.
## Problem Formulation
* *Problem Formulation* is the process of deciding what actions and states to consider, given a goal. 
* **Initial State:** The agent is at location A on the map.
* **State Space:** All possible locations (nodes) on the map that the agent can occupy. 
* **Action:** Move from the current location to any directly connected neighboring location
* **Goal Test:** The agent reaches location B.
### State Search Space (State Space)
The state search space is the set of all possible states that a problem can have, along with the paths between these states caused by valid actions. This includes every situation that the system can be in and all the ways it can move from one situation to another.
#### Components of a State Search Space
* **State:** A specific configuration of the problem.
* **Initial State:** The starting configuration.
* **Goal State:** The desired ending configuration.
* **Successor functions (actions):** Rules that move the system from one state to another. 
* **Path:** Links between states created by applying operators.
## Search
The process of looking for a sequence of actions that reaches the goal is called search. A search algorithm takes a problem as in put and returns a solution in the form of an action sequence.
A state space may be searched in two directions:
* Data Driven Search: From given data towards a Goal
* Goal Driven Search: From a goal back to data
### State Space Search Methods
* Blind/Uninformed/Brute-force Search
* Heuristic/Informed Search 
* Adversarial Search Algorithms (Game Playing)
#### Blind Uninformed Search Methods 
* Breadth First Search (BFS)
* Depth First Search (DFS)
* Iterative Deepening Search (IDS)
* Uniform Cost Search (UCS)
#### Heuristic/Informed Search 
* Best First Search 
* A* Search
#### Adversarial Search Algorithms 
* Minimax Search

### Measuring Problem-Solving Performance
We'll measure the performance of problem solving based on four factors: 
* ***Completeness*** -> Will it find a solution?
* ***Optimality*** -> Will it find the best solution?
* ***Time Complexity*** -> How long will it take?
* ***Space Complexity*** -> How much memory will it use?
## Execution Phase
Once a solution is found, the action it recommends can be carried out and is called the execution phase. 
