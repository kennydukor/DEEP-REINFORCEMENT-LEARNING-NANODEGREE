### Description of the Model Architecture 

The DDPG method was adapted to solve the single agent (version 1) and  20 agent (version 2) environment.

In the algorithm we use the actor and critic (both deep neural networks) to train the model.

- The “Critic” estimates the value function. This could be the action-value (the Q value) or state-value (the V value).
- The “Actor” updates the policy distribution in the direction suggested by the Critic (such as with policy gradients).

Below is the description of the actor and critic architecture
#### Actor

- Input_Layer - (state)
- Hidden_1: (input, 400) - BatchNorm - ReLU
- Hidden_2: (400, 300) - ReLU
- Output: (300, 4) - TanH

#### Critic

- Input_Layer - (state)
- Hidden: (input, 400) - BatchNorm - ReLU
- Hidden: (400 + action_size, 300) - ReLU
- Output: (300, 1) - Linear

### Hyper Parameters

- replay buffer size = int(1e5)
- minibatch size = 128
- discount factor (gamma) = 0.99
- for soft update of target parameters (tau) = 1e-3
- learning rate of the actor = 1e-4
- learning rate of the critic = 1e-4
- L2 weight decay = 0

### Result

The agent reached an average score of 34.10.

<p align="center">
  <img width="660" height="300" src="https://raw.githubusercontent.com/kennydukor/DEEP-REINFORCEMENT-LEARNING-NANODEGREE/master/Collaboration%20and%20Competition/img/episodes.png">
</p>
<p align="center">
  <img width="386" height="266" src="https://raw.githubusercontent.com/kennydukor/DEEP-REINFORCEMENT-LEARNING-NANODEGREE/master/Collaboration%20and%20Competition/img/collaboration_result.png">
</p>


### Future works / Improvement

In order to improve the model further, I intend implementing Prioritised Experience Replay to helps to improve the performance and significantly reduces the training time. [Sum Tree Implementation](https://github.com/rlcode/per)

Also, I intend trying our other reinforcement algorithm for the same problem

- [Asynchronous Actor-Critic Agents (A3C)](https://medium.com/emergent-future/simple-reinforcement-learning-with-tensorflow-part-8-asynchronous-actor-critic-agents-a3c-c88f72a5e9f2)
- [Trust Region Policy Optimisation (TRPO) and Proximal Policy Optimisation (PPO)](https://medium.com/@sanketgujar95/trust-region-policy-optimization-trpo-and-proximal-policy-optimization-ppo-e6e7075f39ed)

- Proximal Policy Optimisation algorithm. [github repository](https://github.com/Cozmo25/drlnd-continuous-control/tree/master/PPO)

