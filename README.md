# Project-Navigation---DRL
A project for training an agent to navigate (and collect bananas) in a large, square world using the Unity Environment

## Project Description
[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif "Trained Agent"

![Trained Agent][image1]

In the simulated environment, a reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

For this project, there are two separate versions of the Unity environment:
- The first version contains a single agent.
- The second version contains 20 identical agents, each with its own copy of the environment.The task is episodic, and in order to solve the environment, our agent must get at least an average score of +13 over 100 consecutive episodes.

In order to solve the environment, the agent must get an average score of +30 over 100 consecutive episodes.
## Getting Started

1. Download the entire repository and unzip (or decompress) the python.taz

2. Place the "python" folder in the working folder.

3. Follow the instructions in `Navigation.ipynb` to get started with training the agent! You can change the hyperparameter as well!

4. You can loading the pretrained model weight by following:
```
agent.qnetwork_local.load_state_dict(torch.load('checkpoint.pth'))
```
## Visualizing Results

The average scores over 2000 iterations:

![plot](result.png)
