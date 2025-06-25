Reinforcement Learning – ViZDoom Basic

A simple Deep Q-Network (DQN) agent trained on the ViZDoom Basic scenario using:

    ✅ Frame stacking (4 grayscale frames)

    ✅ Dueling DQN architecture

    ✅ Experience Replay

    ✅ Double DQN updates

📦 Installation

pip install torch vizdoom opencv-python numpy

Ensure basic.cfg is present in your vizdoom/scenarios directory.
▶️ Run Training


🧩 Components

    ReplayBuffer — manages 4-frame history and sampling

    CNNDQN — convolutional dueling DQN model

    train() — main loop with ε-greedy policy and periodic target network sync

🖼️ Input Format

    Preprocessed grayscale frames

    Resized to 84 × 84

    Stacked as a tensor of shape (4, 84, 84)
