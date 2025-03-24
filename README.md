# Taxi Reinforcement Learning Agent 🚖

This project implements and compares two reinforcement learning algorithms — **Q-learning** and **SARSA** — on the classic **Taxi-v3 environment** from OpenAI Gym. The agent is trained to pick up and drop off passengers as efficiently as possible using a learned Q-table.

---

## Environment

The [Taxi-v3](https://www.gymlibrary.dev/environments/toy_text/taxi/) environment is a grid-based simulation where an agent navigates a map to pick up and drop off passengers at specific locations.

---

## Algorithms Implemented

### 1. Q-learning
- Off-policy algorithm
- Trains a Q-table using the Q-learning update rule to maximise future rewards

### 2. SARSA (State-Action-Reward-State-Action)
- On-policy algorithm
- Updates the Q-table using the reward of the **actual** action taken

Both algorithms are trained over multiple episodes, and performance is measured by the **average number of steps taken to complete an episode**.

---

## Results

- Both agents successfully learned efficient policies.
- Q-learning slightly outperformed SARSA in terms of average episode length.

Pre-trained Q-tables are included:
- `Qlearn_Q_table.npy`
- `SARSA_Q_table.npy`

---

## Repository Structure

```text
├── taxi-v3-rl.ipynb  # Main notebook with code, training, and analysis
├── Qlearn_Q_table.npy                             # Trained Q-table from Q-learning
├── SARSA_Q_table.npy                              # Trained Q-table from SARSA
├── requirements.txt                               # Python dependencies
└── README.md                                      # Project documentation
