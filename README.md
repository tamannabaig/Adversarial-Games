# Adversarial-Games
An Artificial Intelligence Project


This project was created as part of coursework for my Artificial Intelligence course.
The task was to design agents for the deterministic, zero-sum, game Connect Four, in which two players take turns dropping a colored disc from the top into a 7x6 grid. The game is won by forming a horizontal, vertical, or diagonal line of four same colored discs.

The game could be played implementing the following Adversarial algorithms:

<b> Minimax Algorithm: </b>
The minimax function in connect4.py, is to implement depth-limited minimax search. As the game can be played between two agents or an agent and a human player, here Agent1 tis treated as the MAX player and Agent2 or Human as the MIN player. As it's not feasible to search the entire game tree, our code has limited the search to an arbitrary depth by using the GUI. Score the leaves of your minimax tree with the supplied  evaluate function in order to treat them as terminal nodes. 

<b> Alpha Beta Pruning: </b> The alphabeta function in connect4.py uses alpha-beta pruning and allow more efficient exploration of the minimax tree. One should be able to see a speed-up as the depth of the tree increases.  

<b>Expectimax Algorithm: </b> Minimax and alpha-beta assume that MAX plays against an adversary who makes optimal decisions. The expectimax function in connect4.py models a probabilistic behavior of opponents that may make suboptimal decisions. To do so, we would have to replace MIN nodes (Agent2 or Human) with chance nodes. To simplify our code, we assumed yoweu will only be running against an adversary which chooses actions uniformly at random.
