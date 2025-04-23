
# 🐍 Snake Game Reinforcement Learning — Q-Learning vs SARSA

This project implements the classic Snake game using **Reinforcement Learning (RL)** algorithms — **Q-Learning** and **SARSA** — and compares their performance across 500 training episodes.

Agents learn to play Snake autonomously through reward-based interaction, and their behavior is visualized with real-time video and performance graphs.

## 📌 Project Highlights

- ✅ Implemented with **Pygame** and **Python**
- 🧠 Two RL algorithms: **Q-Learning** (off-policy) and **SARSA** (on-policy)
- 📊 Performance comparison through average scores, best scores, and stability
- 🎥 Side-by-side video generation of trained agents
- 📈 Graphical visualization of learning curves


## 🚀 Quick Start

### 1. Clone the Repository
```bash
git clone https://github.com/snehapadgaonkar/SnakeRL.git
cd SnakeRL
```

### 2. Install Dependencies
```bash
pip install pygame numpy imageio matplotlib opencv-python
```

### 3. Run the Notebook
Open `snake_rl.ipynb` in Jupyter or Colab and run all cells to train and evaluate both agents.

## 🤖 Algorithms Overview

| Q-Learning                         | SARSA                              |
|-----------------------------------|------------------------------------|
| Off-policy                        | On-policy                          |
| Uses `max(Q(s', a'))` for update | Uses `Q(s', a')` (actual action)   |
| Faster learning, less stable      | Slower, but more stable behavior   |

> 🔁 Both agents were trained for **500 games** each.

## 📊 Results Summary

| Metric                  | Q-Learning | SARSA     |
|-------------------------|------------|-----------|
| Best Score              | ✅ Higher  | ❌ Lower  |
| Average Score           | ✅ Higher  | ❌ Lower  |
| Cumulative Score        | ❌ Lower   | ✅ Higher |
| Training Time           | ✅ Lower   | ❌ Higher |
| Stability               | ❌ Less    | ✅ More   |

## 🎥 Sample Output

The notebook generates a **side-by-side video** of both agents playing after training and plots a **score graph** over time.

## 📝 References

- Sutton & Barto: *Reinforcement Learning — An Introduction*
- OpenAI Gym (for RL benchmarking environments)
- Python Pygame documentation


## 📌 Future Work

- Implement **Deep Q-Learning (DQN)** using neural networks
- Add state visualization or heatmaps
- Save and load trained Q-tables
