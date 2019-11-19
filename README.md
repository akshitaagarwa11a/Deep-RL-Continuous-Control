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
 
 ## Result
 This solved the environment in 549 episodes.
