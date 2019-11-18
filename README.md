# Deep-RL-Continuous-Control
For this project, I have worked with [Reacher](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#reacher) environment.
## Introduction
![Image](https://video.udacity-data.com/topher/2018/June/5b1ea778_reacher/reacher.gif)</br>
In this environment, a double-jointed arm can move to target locations. 
A reward of +0.1 is provided for each step that the agent's hand is in the goal location.
Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.</br>

The observation space consists of 33 variables corresponding to position, 
rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, 
corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.</br>

**Task:** I have solved the first version in which the task is episodic, and in order to solve the environment, your agent must get an average score of
+30 over 100 consecutive episodes.

## Getting Started

Please follow the [instructions in the DRLND GitHub repository](https://github.com/udacity/deep-reinforcement-learning#dependencies) 
to set up your Python environment. These instructions can be found in ```README.md``` at the root of the repository. 
By following these instructions, you will install PyTorch, the ML-Agents toolkit, and a few more Python packages required 
to complete the project.</br>

(For Windows users) The ML-Agents toolkit supports Windows 10. While it might be possible to run the ML-Agents toolkit using other 
versions of Windows, it has not been tested on other versions. Furthermore, the ML-Agents toolkit has not been tested on a Windows VM 
such as Bootcamp or Parallels.

**Download the Environment**: 
Version 1: One (1) Agent
 - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux.zip)
 - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher.app.zip)
 - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86.zip)
 - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86_64.zip)
 
 ## Running the Code
 Run the Continuous_Control.ipynb file. It uses the model in model.py file and the agent in ddpg_agemt.py file.
 
 ## Model description
 I have used the Actor-Critic method, Deep Deterministic Policy Gradient model to solve the environment.</br>
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
