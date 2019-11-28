## Project: Collaboration and Competition

<p align="center">
  <img width="460" height="300" src="https://video.udacity-data.com/topher/2018/May/5af7955a_tennis/tennis.png">
</p>

### Project Overview
In this environment, two agents control rackets to bounce a ball over a net. If an agent hits the ball over the net, it receives a reward of +0.1. If an agent lets a ball hit the ground or hits the ball out of bounds, it receives a reward of -0.01. Thus, the goal of each agent is to keep the ball in play.

The observation space consists of 8 variables corresponding to the position and velocity of the ball and racket. Each agent receives its own, local observation. Two continuous actions are available, corresponding to movement toward (or away from) the net, and jumping.

The task is episodic, and in order to solve the environment, your agents must get an average score of +0.5 (over 100 consecutive episodes, after taking the maximum over both agents). Specifically,

- After each episode, we add up the rewards that each agent received (without discounting), to get a score for each agent. This yields 2 (potentially different) scores. We then take the maximum of these 2 scores.

- This yields a single score for each episode.

The environment is considered solved, when the average (over 100 episodes) of those scores is at least +0.5.


### Environment Setup

The instructions below describes the procedure required to setup the environment on your own machine! You will also learn how to use the Python API to control your agent.

#### Step 1: Clone the DRLND Repository
---
If you haven't already, please follow the [instructions in the DRLND GitHub repository](https://github.com/udacity/deep-reinforcement-learning#dependencies) to set up your Python environment. These instructions can be found in `README.md` at the root of the repository. By following these instructions, you will install PyTorch, the ML-Agents toolkit, and a few more Python packages required to complete the project on your own.

*(For Windows users)* The ML-Agents toolkit supports Windows 10. While it might be possible to run the ML-Agents toolkit using other versions of Windows, it has not been tested on other versions. Furthermore, the ML-Agents toolkit has not been tested on a Windows VM such as Bootcamp or Parallels.

#### Step 2: Download the Unity Environment
---
For this project, there was no need to install Unity - this is because Udacity built the environment already, and you can be downloaded from one of the links below. You need only select the environment that matches your operating system:

- Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux.zip)
- Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis.app.zip)
- Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86.zip)
- Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86_64.zip)


- Then, place the file in the `p3_navigation/` folder in the DRLND GitHub repository, and unzip (or decompress) the file.

*(For Windows users)* Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

*(For AWS)* If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux_NoVis.zip) to obtain the "headless" version of the environment. You will not be able to watch the agent without enabling a virtual screen, but you will be able to train the agent. *(To watch the agent, you should follow the instructions to [enable a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md), and then download the environment for the Linux operating system above.)*

#### Step 3: Explore the Environment
---
After you have followed the instructions above, open `Tennis.ipynb` (located in the `p3_collab-compet/` folder in the DRLND GitHub repository) and follow the instructions to learn how to use the Python API to control the agent.

### How to Train Agent
Instructions
Follow the instructions in `Tennis.ipynb` to get started with training your own agent!

### Result

#### One (1) Agent
The agent reached an average score of 34.10.

<p align="center">
  <img width="382" height="41" src="https://raw.githubusercontent.com/kennydukor/DEEP-REINFORCEMENT-LEARNING-NANODEGREE/master/Continous%20Control/img/single_agent.JPG">
</p>

#### Twenty (20) Agents
The agents reached an average score of 30.05 after 97 episodes.

<p align="center">
  <img width="441" height="70" src="https://raw.githubusercontent.com/kennydukor/DEEP-REINFORCEMENT-LEARNING-NANODEGREE/master/Continous%20Control/img/multi_agent.JPG">
</p>

### Plot

Score through the episodes

