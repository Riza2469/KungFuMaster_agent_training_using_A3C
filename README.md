# KungFu Master AI Agent Training using A3C  

This repository demonstrates the implementation of an Asynchronous Advantage Actor-Critic (A3C) algorithm to train an AI agent for playing **KungFu Master** in the Atari environment.  

## Description  

The project uses PyTorch for building the neural network and managing the training process. The agent is trained to maximize its performance by learning optimal actions based on states from the game environment.  

## Features  

- **Neural Network Architecture**:  
  - Convolutional layers for feature extraction.  
  - Fully connected layers for policy and value predictions.  

- **Training Highlights**:  
  - Actor-Critic Loss for policy and value updates.  
  - Multi-environment parallel simulation using `EnvBatch`.  
  - Discount factor for long-term reward optimization.  

## Key Parameters  

- **Learning Rate**: 1e-4  
- **Discount Factor**: 0.99  
- **Number of Parallel Environments**: 10  
- **Reward Scaling**: 0.01  

## Training Results  

- The training was conducted for 3001 iterations, using rewards averaged over 10 evaluation episodes at regular intervals.  
- The average rewards during training:  
  - Iteration 0: **780.0**  
  - Iteration 1006: **530.0**  
  - Iteration 2005: **1210.0**  
  - Final Iteration (3001): **1280.0**  

- The agent effectively learned the game mechanics, with performance improving over time.  

### Training Logs  

```text  
Iteration 0: Average Agent Reward: 780.0  
Iteration 1006: Average Agent Reward: 530.0  
Iteration 2005: Average Agent Reward: 1210.0  
Iteration 3001: Average Agent Reward: 1280.0  
```  

## Video Demonstration  

A sample video of the trained AI agent playing **KungFu Master** is included

## How to Run  

### Prerequisites  

- Python 3.10 or above  
- PyTorch 1.9+  
- Gymnasium  
