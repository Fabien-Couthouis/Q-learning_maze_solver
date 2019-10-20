# RL-maze-solver

The goal here is to implement a Reinforcement Learning algorithm: Q-learning to solve a randomly generated maze.

## Description 
An robot/agent can move in a m*n maze. The environment can have a random component: with each choice of movement (up, down, left or right), the agent can move in an unwanted direction. This behavior is configurable.

It is assumed that the environment is fixed: the position of the elements will not be changed between each part. It is therefore a matter of learning the structure of the ground, to be able to move the agent correctly.

The code provides Q-learning implementation with Q-table and with a simple neural network.

## Usage
The code provided in the notbook can be used like this:
```python
game = Game(n=8,m=8,nb_blocks=15)
agent = Agent(game, use_nn=True)
agent.train(num_episodes=100)
```

## Credits
Based on [Akka Zemmari](https://www.labri.fr/perso/zemmari/) RL courses at [ENSEIRB-MATMECA](https://enseirb-matmeca.bordeaux-inp.fr/fr)