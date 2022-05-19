# Model-Based Reinforcement Learning
This repository provides a tensorflow implementation of Model-based reinforcement learning for ***CartPole*** environment. This repo also aims at helping beginners in [Reinforcement Learning](https://en.wikipedia.org/wiki/Reinforcement_learning) to better understand how to train the agent using the model rather than requiring to use the real environment every time in order to learn the dynamics of the real environment space.
A concise explaination of Model-based reinforcement learning algorithm can be found [here](https://medium.com/@awjuliani/simple-reinforcement-learning-with-tensorflow-part-3-model-based-rl-9a6fe0cce99).
## Requirements
- `tensorflow`
- `matplotlib`
- `numpy`
## Training Environment Used
- `OpenAI Gym's CartPole-v1 Environment`
## Usage
- `Model_based_RL.py` file contains code statements related to ***Model Network*** and ***Policy Network*** that are being used here.
- The training procedure involves switching between training the ***Model Network*** using the real environment, and training the agent’s policy using the model environment. By using this approach, the ***Model Network*** will be able to learn a policy that allows the trained agent to solve the ***CartPole*** task without actually ever training the policy on the real environment.
- All hyperparameters to train the two networks can be found in `Model_based_RL.py`.
- The *episode number, action, reward and mean reward* are printed after very epoch during training time.
## Results
| CartPole-v1 Environment        | CartPole-v1 Results           |
| ------------------------------ |:-----------------------------:|
| ![alt text](https://github.com/fork123aniket/Model-Based-Reinforcement-Learning/blob/main/Images/CartPole-v1.gif) | ![alt text](https://github.com/fork123aniket/Model-Based-Reinforcement-Learning/blob/main/Images/Result.PNG) |
