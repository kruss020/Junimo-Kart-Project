# Junimo Kart Reinforcement Learning

## Overview
A reinforcement learning project comparing Double Deep Q-Networks (DDQN) and Proximal Policy Optimization (PPO) on a custom Gymnasium environment inspired by Junimo Kart from Stardew Valley.

## Features
- Custom Gymnasium environment
- Procedural terrain generation
- Custom platforming physics
- CNN + MLP hybrid neural network
- DDQN implementation
- PPO implementation
- Training visualizations
- Gameplay rendering

## Results
DDQN consistently outperformed PPO on this sparse-reward platformer environment, achieving higher average returns and more stable learning.

## Technologies
- Python
- PyTorch
- Gymnasium
- NumPy
- Matplotlib
- Pygame

## Repository Structure

```text
Junimo-Kart-Project/
│
├── README.md
│   Project overview, setup instructions, and repository documentation.
│
├── CS258_Final_Report.pdf
│   Comprehensive report describing the motivation, environment design,
│   reinforcement learning methodology, experimental results, and conclusions.
│
├── JunimoKart.ipynb
│   Main project notebook containing the complete implementation of the
│   custom Gymnasium environment, PPO and DDQN agents, training pipeline,
│   evaluation, visualization, and gameplay rendering.
│
├── ddqn_network.pth
│   Saved weights for the trained Double Deep Q-Network (DDQN) model.
│
├── ppo_policy.pth
│   Saved weights for the trained PPO policy network.
│
├── ppo_value.pth
│   Saved weights for the trained PPO value network.
│
├── ddqn_video.mp4
│   Gameplay demonstration of the trained DDQN agent.
│
├── ppo_policy_video.mp4
│   Gameplay demonstration of the trained PPO agent.
│
├── junimo_kart_demo.mp4
│   Gameplay using random actions, included as a baseline comparison
│   to demonstrate the learning achieved by the trained agents.
│
├── ddqn_model/
│   Training results for the DDQN agent, including the saved model,
│   evaluation return curves, score curves, and a successful gameplay run.
│
├── ppo_model/
│   Training results for the PPO agent, including the saved policy and
│   value networks, evaluation return curves, score curves, and a
│   successful gameplay run.
│
├── Files For Presentation/
│   Presentation slides and presentation video prepared for the course.
│   These materials primarily discuss the PPO implementation, as the
│   DDQN agent was completed later and ultimately achieved stronger results.
│
└── assets/
    Custom 24×24 pixel art sprites used throughout the environment,
    including terrain tiles, collectibles, obstacles, and other game assets.
```

### Main Components

- **Custom Gymnasium Environment** – A procedurally generated side-scrolling platformer inspired by the *Junimo Kart* minigame from *Stardew Valley*.
- **DDQN Implementation** – Custom implementation of Double Deep Q-Networks used for training and evaluation.
- **PPO Implementation** – Custom implementation of Proximal Policy Optimization for comparison against DDQN.
- **Training Results** – Saved models, training curves, evaluation metrics, and gameplay demonstrations for both reinforcement learning algorithms.
- **Presentation Materials** – Slides and presentation video explaining the project's design and methodology.
- **Custom Assets** – Original pixel art sprites created specifically for the environment.
- **Final Report** – Detailed documentation covering the environment, methodology, experiments, implementation challenges, and conclusions.

## Final Report

A detailed write-up of the project, including the environment design, methodology, experiments, and results, is available in **CS258_Final_Report.pdf**.

## Installation

Clone the repository:

```bash
git clone https://github.com/kruss020/Junimo-Kart-Project.git
cd Junimo-Kart-Project
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Open **JunimoKart.ipynb** in Jupyter Notebook or JupyterLab to train, evaluate, or visualize the reinforcement learning agents.

## Future Work

Possible extensions include:
- Implementing additional RL algorithms such as SAC and DDPG.
- Applying imitation learning or behavioral cloning.
- Performing hyperparameter optimization and reward shaping experiments.
- Expanding the environment with additional levels and mechanics
