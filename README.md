# Reinforcement-Learning-vizdoom-game-environment

Reinforcement Learning in ViZDoom

A simple Deep Q-Learning agent trained to play the ViZDoom Basic scenario using:

    Frame stacking (4 grayscale frames)

    Dueling DQN architecture

    Experience Replay

    Double DQN target updates

📦 Requirements

pip install torch vizdoom opencv-python numpy

▶️ Run Training

from train import train
train()

Ensure the basic.cfg scenario is available in your vizdoom.scenarios_path.
🧠 Key Components

    ReplayBuffer: handles 4-frame stacking and sampling

    CNNDQN: convolutional dueling architecture

    train(): main loop with epsilon-greedy policy and target net sync

🖼️ Input Format

    Grayscale frames

    Resized to (84, 84)

    Stacked as shape (4, 84, 84)
