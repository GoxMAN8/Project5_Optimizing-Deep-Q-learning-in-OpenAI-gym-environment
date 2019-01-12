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



