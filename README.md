# Project5_Optimizing-Deep-Q-learning-in-OpenAI-gym-environment

Project part of the module INM426, Software Agents, City University, London. Synthesis of a full report.

# Definition of the problem 

OpenAI gym provides the main public environment to train reinforcement learning (RL) agents. Content of the gym, involves Atari2600 game environments, along with more recent basic human movement, and robotic hand control environments. A big breakthrough in reinforcement learning occurred with the publishing of 2013 paper, 
by DeepMind technologies in which they used an Artificial Neural Network as a Q matrix approximator. 
This technique is the most beneficial when the problem is high dimensional. 
Their learner was able to surpass any previous approach on 6 Atari2600 environments, and achieved superhuman level on 3 of them.
In this paper, our goal is to solve the ‘LunarLander-v2’ environment, using deep-Q learning. 
The goal of this mini game is to land the Lunar Lander on its two feet, between the two flags, after it is being dropped into the environment. 
There are 4 actions available: fire left, right or main engines or do nothing. 
The game episode ends when Lander crashes, lands or flies away from the environment coordinate system.


# Workflow

1. Data

Environment is ready and available at https://gym.openai.com/. Game is ‘LunarLander-v2’. 

2. Optimization and analysis

In order to find the best possible learning model for our software agent, we have employed a grid search for 
the following parameters: discount rate (0.1; 0.5, 0.9); exploration decay (0.1; 0.5; 0.99) and rate (0.1; 0.5;0.9); learning rate (0.0001;0.01). 

Agent is improved using best parameters from grid-search, and optimizing two neural net parameters – activation function (ReLU; LeakyReLU; Sigmoid) and number of nodes in hidden layers (6; 25; 50).

3. Conclusions

In this paper, Deep Q learning algorithm to train an agent in a discrete space was used. It was determined that it preformed best with base parameters, high exploration and exploration decay rates (0.8, 0.99); low learning rate (0.00025); high discount rate (0.9); 30 nodes in each of two hidden layers in action-value approximator, and ReLU activation functions. Understanding what agent does to land the Lunar Lander in the correct position, could be useful for modelling a real life drone or an experimental space rocket.
