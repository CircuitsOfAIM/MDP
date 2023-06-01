## Markov Decision process (MDP) implementation in a grid world using value iteration

an agent navigating a 2D, discrete environment (a grid).
The cells of the grid, depicted below, correspond to the states of the environment.
At each cell, 4 actions are possible: `north`, `south`, `east` and `west`.
These actions move the agent in the corresponding direction. There are 2 special states `A` and `B`,
from which any action always pushes the agent to states `A'` and `B'`, respectively.
This special transition also results in larger rewards (+10 and +5, respectively).
Actions that would take the agent off the grid have no effect (the agent remains in the same position) and result in a reward of -1.
Other actions result in 0 reward.

Agent selects all four actions with equal probability in all states and random uniform policy with a discounting factor $\gamma = 0.9$ is assumed.

This code computes compute state-value functions by value iteration and
the direct solution of the linear Bellman equations for this problem.

<img alt="Grid world MDP" height="300" src="https://drive.google.com/uc?id=1Wx6ALilXFkkRG5scC4r8h0U--qffgt9s" title="Grid World" width="500"/>
Reference:Sutton & Barto, Ch.3, p.60 (example 3.5)


**Note** : This is a simple MDP implementation exercsie related to the Reinforcement learning course at Radboud University.All rights are reserved.
