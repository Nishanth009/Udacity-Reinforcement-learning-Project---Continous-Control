# Udacity-Nano-Degree-RL-Project-Navigation

![](/images/reacher.gif)

## Project Details

The project solves reacher environment by using ddpg algorithm.In this environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector will be a number between -1 and 1.

20 identical agents are trained to perform the task

## Getting Started


Install anaconda(python package manager)-python 3, then run ./install.sh file.This will install unity ml-agents, torch and other neccessery libraries


## Instructions

Run **Continous_control.ipynb**. Agent uses DDPG for training and must get an average score of +30 (over 100 consecutive episodes, and over all agents) to solve the environment
Check **REPORT.md** for results and agents performance
