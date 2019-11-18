# Implementation Details
I have used the Actor-Critic method, Deep Deterministic Policy Gradient model to solve the environment.</br>
## Model description
I have used 2 hidden layers with 512 and 256 hidden units for both actor and critic.</br>
 **Hyperparameters**:</br>
 - BUFFER_SIZE = int(1e6)  # replay buffer size
 - BATCH_SIZE = 128        # minibatch size
 - GAMMA = 0.99            # discount factor
 - TAU = 0.125              # for soft update of target parameters
 - LR_ACTOR = 1e-3         # learning rate of the actor
 - LR_CRITIC = 1e-3        # learning rate of the critic
 - WEIGHT_DECAY = 0        # L2 weight decay
 - LEARN_EVERY = 20        # learning timestep interval
 - LEARN_NUM   = 10        # number of learning passes
 - GRAD_CLIPPING = 1.0     # Gradient Clipping
#Ornstein-Uhlenbeck noise parameters
 - OU_SIGMA  = 0.15
 - OU_THETA  = 0.05
 
 - EPSILON       = 1.0     # for epsilon in the noise process (act step)
 - EPSILON_DECAY = 1e-6
 
 ## Result
 This solved the environment in ___ episodes.
## Future Scope
Here's a list of optimizations that can be applied to the project:

- Build an agent that finds the best hyperparameters for an agent
- Prioritization for replay buffer
- Paramter space noise for better exploration
- Test shared network between agents
- Test separate replay buffer for agents
