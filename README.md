## Deep Q Learning to classify Bearing Fault Modes using Continous Wavelet Transform Scalograms

### RL Scheme

![](https://github.com/Shrav108/DQN-for-Bearing-Fault/blob/main/Pictures/RL%20Scheme.PNG).


### Episode
1. One episode is basically a set of scalogram images of bearing faults. 
2. The Question to the agent when looking at an image is "To which fault does the scalogram belong to ?"

![](https://github.com/Shrav108/DQN-for-Bearing-Fault/blob/main/Pictures/Quiz.PNG)


### RL Training




#### Description:
1. In this project, bearing fault classification is done with the help of Deep Q Learning method.
2. A Deep Reinforcement Learning Agent is used to predict whether vibration data of a bearing state is in
   which fualt mode.
3. The deep reinforcement learning agent has a 2 Convolution Layer with 2 Fully connected layers and a output 
   layer to predict q-values.
4. Vibration data is converted to 2D Continous Wavelet Transform Scalogram for the Training and Testing the               agent.
5. The training takes place as quiz game where the agent will predict N number of scalograms in an episode. 
   The scalograms in an episode contains Bearing state of 4 different conditions.
6. If the agent predicts correctly, then it gets a reward of +1 else -1.
7. The goal of the agent is to maximize rewards, thus the goal is to train the agent to predict the state of 
   the scalogram.


#### Reference Paper: 
                 Intelligent fault diagnosis for rotating machinery using deep Q-network
                 based health state classification: A deep reinforcement learning approach by:
                 Yu Ding, Liang Ma, Jian Ma, Mingliang Suo, Laifa Tao, Yujie Cheng, Chen Lu

#### Data: Case Western Bearing Data
      https://engineering.case.edu/bearingdatacenter/download-data-file
      
