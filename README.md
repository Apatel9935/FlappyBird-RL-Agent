# Flappy Bird AI using Deep Reinforcement Learning

A Deep Reinforcement Learning project where an AI agent learns to play Flappy Bird using Deep Q Networks (DQN) implemented in PyTorch.

---

## Project Overview

This project trains an autonomous agent to play Flappy Bird using Reinforcement Learning techniques instead of traditional supervised learning.

The agent interacts with the environment, collects experiences, learns optimal actions using Q-learning, and gradually improves gameplay performance over time.

---

## Features

- Deep Q Network (DQN)
- Experience Replay Memory
- Epsilon-Greedy Exploration Strategy
- Target Network Synchronization
- Training and Testing Modes
- Model Checkpoint Saving
- Reward Logging System
- GPU/CPU Device Support

---

## Technologies Used

- Python
- PyTorch
- Gymnasium
- Flappy Bird Gymnasium
- Reinforcement Learning

---

## Project Structure

```bash
FLAPPYRL/
│
├── agent.py
├── dqn.py
├── experience_replay.py
├── parameters.yaml
├── README.md
└── .gitignore
```

---

## Reinforcement Learning Concepts Used

### Deep Q Network (DQN)

A neural network approximates the Q-value function to predict the best action for a given state.

### Experience Replay

Past experiences are stored and randomly sampled during training to improve stability and learning efficiency.

### Epsilon-Greedy Policy

The agent balances:
- Exploration → random actions
- Exploitation → best predicted actions

### Target Network

A separate target network is periodically synchronized to stabilize training.

---

## Training Process

The agent:
1. Observes game state
2. Selects an action
3. Receives reward
4. Stores experience in replay memory
5. Samples mini-batches
6. Updates Q-network using gradient descent

---

## Run the Project

### Train the Agent

```bash
python agent.py flappybirdv0 --train
```

### Test the Trained Model

```bash
python agent.py flappybirdv0
```

---

## Author

Akshat Patel  
B.Tech Electronics and Communication Engineering  
Madan Mohan Malaviya University of Technology

---

## Project Goal

This project was built to explore Deep Reinforcement Learning and understand how intelligent agents learn through interaction with environments.