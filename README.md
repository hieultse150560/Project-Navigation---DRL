# Project-Navigation---DRL
A project for training an agent to navigate (and collect bananas) in a large, square world using the Unity Environment

## Project Description
[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif "Trained Agent"

![Trained Agent][image1]

In the simulated environment, the agent will get the reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana.  Thus, the goal of the agent is to collect as many yellow bananas as possible while avoiding blue bananas.  

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction.  Given this information, the agent has to learn how to best select actions.  Four discrete actions are available, corresponding to:
- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

The task is episodic, and in order to solve the environment, our agent must get at least an average score of +13 over 100 consecutive episodes.

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
