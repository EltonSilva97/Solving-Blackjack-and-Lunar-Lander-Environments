# Reinforcement Learning Project – Blackjack & Lunar Lander
**Author:** Elton Silva

## Overview
This project applies and compares reinforcement learning algorithms across two environments using the OpenAI Gym interface:
- **Blackjack** (discrete environment)
- **Lunar Lander** (continuous environment)

## Implemented algorithms
**Blackjack:**
- Double Q-Learning
- Expected SARSA

**Lunar Lander:**
- Proximal Policy Optimization (PPO)
- Soft Actor-Critic (SAC)

File Structure
RL Project/
│
├── Blackjack.ipynb                         # Tabular methods for Blackjack
├── Lunar Lander.ipynb                      # PPO and SAC implementations
│
├── sac_lunarlander_actor.pt                # Trained SAC actor model
├── sac_lunarlander_critic.pt              # Trained SAC critic model
├── ppo_lunarlander_final.pt               # Trained PPO model


How to Run
You can run the notebooks directly using Jupyter:
```bash
jupyter notebook
```

Open either:
Blackjack.ipynb for tabular RL
Lunar Lander.ipynb for PPO and SAC
Each notebook includes all the training loops, hyperparameters, training logs, and visualizations.

## Highlights
**Blackjack:**
- Double Q-Learning reduces overestimation bias by decoupling action selection and evaluation.
- Expected SARSA improves convergence stability by using expected next-state values.
- Value functions are visualized as heatmaps.

**Lunar Lander:**
- PPO uses clipped surrogate objectives for stability.
- SAC integrates entropy maximization to improve exploration.
- Saved models (.pt files) can be reused for testing and evaluation.

## Visualization
**Blackjack:**
- Reward curves
- Action Probabilities
- Convergence Analysis with confidence intervals
- State-value functions (Blackjack)

**Lunar Lander:**
- Reward curves
- Rolling Standard Deviation
- Learning Velocity
- Return vs Episode Length
- Cumular Rewards over time

## Requirements
**Tested with:**
- Python 3.10.18
- Jupyter
- PyTorch
- Gym
- Matplotlib
- Seaborn
- NumPy
- Pygame
- SciPy
