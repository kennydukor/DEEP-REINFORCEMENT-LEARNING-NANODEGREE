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
