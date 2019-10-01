## Project: Navigation 

<p align="center">
  <img width="460" height="300" src="https://video.udacity-data.com/topher/2018/June/5b1ab4b0_banana/banana.gif">
</p>

#### Project Overview
In this project, I trained an agent to navigate (and collect bananas!) in a large, square world.

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of the agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:

- 0 - move forward.
- 1 - move backward.
- 2 - turn left.
- 3 - turn right.
The task is episodic, and in order to solve the environment, the agent must get an average score of +13 over 100 consecutive episodes.

#### Result

The agent reached an average score of +13 after 369 episodes in 9.8 minutes.

<p align="center">
  <img width="460" height="300" src="https://raw.githubusercontent.com/kennydukor/DEEP-REINFORCEMENT-LEARNING-NANODEGREE/master/Navigation%20Project/number_episodes.jpg">
</p>

#### Plot

Score through the episodes
<p align="center">
  <img width="460" height="300" src="https://raw.githubusercontent.com/kennydukor/DEEP-REINFORCEMENT-LEARNING-NANODEGREE/master/Navigation%20Project/plot.jpg">
</p>
