# snake-game-rl

A reinforcement learning Python project that teaches an AI to play Snake using Q-learning.

## Installation

1. Clone the repository:

```bash
git clone https://github.com/QwertyuiopIsTaken/snake-game-rl.git
```

2. Install dependencies:

```bash
pip install matplotlib numpy torch pygame 

```

3. Run the program:

```bash
python -m scripts.train
```

## How it works

The agent learns optimal actions using the Bellman equation and updates Q-values based on rewards.

To improve on the original state representation, I added directional distances between snake parts to prevent long snakes from trapping itself.

You can turn the render off in `train/train.py`

```python
game = SnakeGameAI(render=False)
```

to increase simulation speed.

<p align="center">
    <img src=https://github.com/QwertyuiopIsTaken/snake-game-rl/blob/main/assets/example-graph.png alt="Score vs runs graph of a model training simulation" width="800" height="800">
</p>

## Warnings

This project should be run with Python 3.12. Unfortunately, PyGame does not currently support Python 3.14+. You can install Python 3.12 [here](https://www.python.org/downloads/release/python-3120/) and make sure to check "Add Python to PATH" during installation.

## Credits

This project is based on a reinforcement learning tutorial by Patrick Loeber in his YouTube playlist [Teach AI To Play Snake](https://www.youtube.com/watch?v=PJl4iabBEz0&list=PLqnslRFeH2UrDh7vUmJ60YrmWd64mTTKV).

