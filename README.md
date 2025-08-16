# Multi-armed-bandit-epsilon-greedy
This repository presents the implementation, simulation, and analysis of the Epsilon-Greedy algorithm for solving the Multi-Armed Bandit (MAB) problem

The Multi-Armed Bandit problem is a fundamental challenge in **reinforcement learning**, where an agent repeatedly chooses from multiple actions (“arms”) to maximize cumulative rewards. The difficulty lies in balancing **exploration**—testing new actions to discover their potential rewards—and **exploitation**—leveraging the best-known actions for immediate gain.

The project implements the **Epsilon-Greedy strategy**, a widely used approach where the agent selects a random action with probability *ε* (exploration) and the best-known action with probability *(1–ε)* (exploitation). This balance ensures that the agent continues learning about less-tried options while capitalizing on high-reward actions.

### Key Features
- **Simulation Setup:** 2000 bandit tasks, each with 10 arms, run for 2000 iterations.
- **Performance Tracking:** Average reward progression and percentage of optimal actions over time.
- **Action-Value Methods:**
  - **Sample-Average Method** – Updates action values by averaging received rewards.
  - **Incremental Update Method** – Updates action values incrementally using a step-size parameter.
  - **Q-Learning** – Stores and updates action values in a Q-table for reinforcement learning tasks.

### Results
The results show that over time, the Epsilon-Greedy approach significantly increases both the average rewards and the percentage of optimal actions selected. Plots indicate that the percentage of optimal actions stabilizes at around 65% after 2000 plays, highlighting the trade-off between exploration and exploitation.
