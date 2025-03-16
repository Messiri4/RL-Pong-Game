# Reinforcement Learning Pong Game
Train AI to play Pong

## Overview

This project implements a Deep Q-Network (DQN) to train an agent to play Atari games using OpenAI Gymnasium. The model is designed to learn optimal policies through reinforcement learning techniques.

## Dependencies

Ensure you have the following dependencies installed before running the notebook:

```sh
pip install numpy matplotlib torch gymnasium[atari,accept-rom-license] ale-py autorom[accept-rom-license] atari_py pyvirtualdisplay
apt-get install -y xvfb
```

## Project Structure

The notebook is structured as follows:

1. **Install Dependencies**: Installs necessary Python libraries.
2. **Setup and Initialization**: Imports required libraries and initializes the environment.
3. **Define the Neural Network**: Implements a Convolutional Neural Network (CNN) as the policy model for reinforcement learning.
4. **Experience Replay**: Utilizes a replay buffer to store past experiences and improve training stability.
5. **Training the Agent**: Implements the reinforcement learning loop, training the agent to optimize its gameplay.
6. **Evaluation**: Tests the trained model's performance and visualizes the results.

## Running the Notebook

1. Open the Jupyter Notebook (`RL_Pong.ipynb`).
2. Run each cell sequentially to install dependencies, set up the environment, define the model, and train the agent.
3. Monitor the training process and evaluate the agent's performance at the end.

## Expected Outcome

By the end of training, the agent should demonstrate improved gameplay performance based on the learned Q-values.

## Troubleshooting

- If the environment does not load, ensure you have installed `ale-py` and `atari_py` correctly.
- If the training is slow, consider reducing the number of episodes or adjusting the batch size.
- Ensure your Python and library versions are compatible with the Gymnasium API.

## Future Improvements

- Implement Double DQN to reduce overestimation bias.
- Use a Prioritized Experience Replay buffer for better learning efficiency.
- Train on multiple Atari games to generalize learning.
