# The Pacman Game with Q-Learning

## Solving the Pacman Game with Q-Learning

### Introduction
In this project, we will learn how to solve the Pacman game using Q-learning. The environment consists of agents, dots, walls, and optional ghosts (adding ghosts will provide bonus points). To discretize and digitize the paths, we convert them into small unit squares. The starting point of the agent’s movement is also predetermined. The goal is to collect all the dots in the environment without encountering any ghosts (the agent cannot pass through walls). 

In the figure below:
- **W** stands for wall
- **A** stands for agent
- **D** stands for dot
- **G** stands for ghost
- **E** stands for empty cell (a cell becomes empty after the agent collects the dot).

<img width="673" alt="Screenshot 1403-07-24 at 12 46 21" src="https://github.com/user-attachments/assets/978290be-7f8e-4e51-8a8e-89886c3a51d9">

### Q-Learning Overview
Q-learning is a model-free reinforcement learning algorithm that enables agents to learn optimal action-selection policies through interaction with their environment. In the context of the Pacman game, the agent learns to navigate the grid, collect dots, and avoid ghosts by estimating the value of taking specific actions in various states. 

1. **Q-Value Function**: The algorithm maintains a Q-table that represents the expected future rewards for each action taken in each state. The agent updates its Q-values based on the rewards received and the estimated future rewards, guiding its decision-making process.

2. **Exploration and Exploitation**: To balance exploration of new actions and exploitation of known rewarding actions, the agent employs strategies like ε-greedy, where it occasionally chooses a random action to discover potentially better strategies.

3. **Learning Process**: The agent iteratively interacts with the environment, updating its Q-values using the Q-learning update rule. As the agent continues to explore and gather experiences, it converges towards an optimal policy that maximizes the collection of dots while avoiding ghosts.

By applying Q-learning to the Pacman game, we aim to develop a robust AI that efficiently collects dots while navigating the challenges of the game environment.
