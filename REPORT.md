# Project: Continous Control

In this environment, we train a set of agents to move their hand to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your the agent is to maintain its position at the target location for as many time steps as possible.

## Environment 

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.
Agents must get an average score of +30 (over 100 consecutive episodes, and over all agents) to solve the environment

## Learning Algorithm

The environment is solved using Deep Deterministic Policy Gradients, an actor-critic algorithm. DDPG helps to solves this task in less episodes as well as it works with continous action space. 

### Deep learning model architecture:-<br>

Algorithm uses two networks one for Actor and one for Critic

Actor: 64->128<br>
Critic: 64 -> 128

### Hyperparameters:-
BUFFER_SIZE = int(1e5)  # replay buffer size   <br>
BATCH_SIZE = 128        # minibatch size       <br> 
GAMMA = 0.99            # discount factor      <br>
TAU = 1e-3              # for soft update of target parameters <br>
LR_ACTOR = 1e-4         # learning rate of the actor           <br>
LR_CRITIC = 1e-4        # learning rate of the critic          <br>
WEIGHT_DECAY = 0        # L2 weight decay                      <br>

 
## Plot of score vs episodes(training)
![](/images/reacher.png)
<br>
Environment is solved in 135 episodes with an average Score of 30.19<br>
Weights file: **checkpoint_actor.pth, checkpoint_critic.pth**

## Ideas for Future Work

1) Try various hyperparameters and observe how it effects the agents performance
2) Try different network architecture
3) Use a different learning algorithm PPO or A2C

