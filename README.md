# CartPole Policy Gradient (Reinforcement Learning)

## Overview
This project implements a Policy Gradient reinforcement learning algorithm to solve the CartPole environment from OpenAI Gym. The agent learns to balance a pole on a moving cart by optimizing its policy based on rewards received from the environment.

The notebook demonstrates how neural networks can be trained using policy-based methods instead of value-based approaches like Q-learning.

---

## Features
- Policy Gradient (REINFORCE) implementation  
- Neural network-based policy model  
- Episodic training with reward-based updates  
- Visualization of training performance  
- Works with OpenAI Gym CartPole environment  

---

## Environment
- CartPole-v1 (OpenAI Gym)
- Objective: Keep the pole balanced by moving the cart left or right
- Reward: +1 for every timestep the pole remains upright

---

## Installation

### Clone Repository
git clone <your-repo-link>  
cd cartpole-policy-gradient  

### Install Dependencies
pip install numpy matplotlib torch gym  

---

## Usage

1. Open the notebook:
   jupyter notebook CartPole_PolicyGradient.ipynb  

2. Run all cells sequentially  

3. The agent will:
   - Interact with the environment  
   - Collect rewards  
   - Update its policy  
   - Improve performance over episodes  

---

## How It Works

### Step 1: Initialize Policy Network
A neural network maps states to action probabilities.

### Step 2: Collect Trajectories
- Agent interacts with environment
- Stores states, actions, and rewards

### Step 3: Compute Returns
- Discounted rewards are calculated for each timestep

### Step 4: Policy Update
- Apply REINFORCE algorithm
- Update weights using gradient ascent on expected reward

---

## Model Details
- Input: State space (cart position, velocity, pole angle, angular velocity)
- Output: Probability distribution over actions (left/right)
- Loss: Negative log-likelihood weighted by returns

---

## Results
- The agent learns to balance the pole over time
- Episode rewards increase as training progresses
- Converges to near-optimal performance with sufficient training

---

## File Structure
├── CartPole_PolicyGradient.ipynb  
├── README.md  

---

## Future Improvements
- Add baseline to reduce variance (Advantage Actor-Critic)  
- Implement entropy regularization  
- Extend to continuous action spaces  
- Compare with DQN and PPO  

---

## Use Cases
- Learning reinforcement learning fundamentals  
- Understanding policy gradient methods  
- Experimenting with neural network-based agents  

---

## Author
Kritika Vyas  

---

## License
This project is for educational purposes.
