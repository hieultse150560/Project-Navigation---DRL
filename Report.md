In this project, I utilized the the Double Deep Q-Network, or Double DQN to reduce overestimation by decomposing the max operation in the target into action selection and action evaluation. 
The motivation behind the Double Q-Network is that we evaluating the greedy policy according to the online network, but we also use the target network to estimate its value. 
The update is the same as for DQN, but replacing the target $Y_{t}^{DQN}$ with:

 $$Y_{t}^{DoubleDQN} = R_{t+1} + \gamma $$ 

Compared to the original formulation of Double Q-Learning, in Double DQN the weights of the second network are replaced with the weights of the target network for the evaluation of the current greedy policy.
