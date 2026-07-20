# Reward Engineering for Reinforcement Learning-based Autonomous Maze Navigation
![Reinforcement Learning](https://img.shields.io/badge/Reinforcement-Learning-green)
![Robotics](https://img.shields.io/badge/Robotics-Autonomous-orange)
![Hackathon](https://img.shields.io/badge/Hackathon-CSE%20SummerSchool%202026-red)
![Portfolio](https://img.shields.io/badge/Portfolio-Project-purple)

A Reinforcement Learning (RL) policy optimization project developed during a robotics hackathon, focusing on autonomous robot navigation in a simulated maze environment.

Instead of modifying the learning algorithm itself, our team focused on **reward engineering** to improve the agent's navigation behaviour through iterative experimentation and policy refinement.

<img width="854" height="855" alt="image" src="https://github.com/user-attachments/assets/1e078e78-8828-46ba-a65d-fc04afccdf25" />


---

## Team

| Member | Responsibilities |
|---------|------------------|
| **Phan Hong Phuc** | Reward engineering, policy optimization, presentation (Objective 2: Coverage) |
| **Nguyen Chi Nguyen** | Reward engineering, policy optimization, presentation (Objective 1: Checkpoints) |
| **Dao Cong Tri Bao** | Reward engineering, policy optimization, presentation (Objective 2: Coverage) |
| **Tran Hoang Son** | Reward engineering, policy optimization, presentation (Objective 3: Wall-touching) |
| **Nguyen Hoang Khang Huy** | Reward engineering, policy optimization, presentation (Objective 3: Wall-touching) |

Mentor: **Nguyen Minh Thai** (VNUHCM - Ho Chi Minh City University of Technology)

---

# Project Overview

## Objective

Improve the navigation policy of an autonomous robot operating inside randomly generated maze environments by designing an effective reward function.

The optimized policy aims to:

- Reach the goal efficiently
- Collect checkpoints
- Maximize map coverage
- Avoid wall collisions
- Reduce unnecessary movements
- Balance exploration and exploitation

---

# Environment

The simulator and training environment were provided exclusively by the hackathon organizers.

The environment includes:

- Randomly generated maze maps
- Autonomous robot agent
- Obstacles and walls
- Goal position
- Checkpoints
- Reward-based Reinforcement Learning framework

> **Note**
>
> The simulator is proprietary and cannot be publicly distributed.
> Therefore, this repository documents our engineering methodology, experimental process, and project outcomes rather than the simulator source code.

---

# Engineering Approach

Rather than changing the RL algorithm itself, our team focused on **reward shaping**.

We iteratively modified reward functions, trained the agent, observed its behaviour, identified failure cases, and refined the policy until achieving stable navigation performance.

The optimization process primarily targeted three objectives:

- Objective 1 — Checkpoint Collection
- Objective 2 — Map Coverage
- Objective 3 — Wall-touching

---

# Reward Policy

One of the reward configurations evaluated during experimentation:

| Event | Reward |
|--------|-------:|
| Reach Goal | +400 |
| Reach Checkpoint | +100 |
| Collision | -200 |
| Every Action | -2 |

The reward function was continuously refined to improve:

- Navigation efficiency
- Policy stability
- Collision avoidance
- Exploration strategy

---

# Experiments

Multiple reward configurations were evaluated through repeated training and inference.

Evaluation focused on:

- Goal-reaching behaviour
- Checkpoint collection
- Coverage efficiency
- Collision frequency
- Navigation stability

The final policy was evaluated on **500+ randomly generated maze maps**.

---

# Engineering Challenges

Some common failure cases encountered during policy optimization included:

- Robot repeatedly colliding with walls
- Robot spinning in place until reaching the maximum step limit
- Inefficient exploration resulting in poor map coverage

These behaviours were gradually reduced through reward engineering and iterative experimentation.

---

# Results

The optimized reward policy demonstrated:

- Stable navigation across 500+ generated maps
- More consistent goal-reaching behaviour
- Improved exploration efficiency
- Reduced collisions
- Better balance between exploration and exploitation

---

# Lessons Learned

Through this project we learned that:

- Reward engineering plays a critical role in Reinforcement Learning.
- Good performance depends on balancing reward design, training episodes, and training map diversity.
- The training environment is just as important as the learning algorithm itself.
- Policy optimization is an iterative engineering process rather than a one-time tuning task.

---

# Tech Stack

- Reinforcement Learning
- Reward Engineering
- Autonomous Navigation
- GitHub

*(Simulation platform provided by the organizers.)*

---

# Repository Structure

```
.
├── README.md
├── LICENSE.md
├── docs/
│   ├── Final_Presentation.pdf
│
├── images/
│   ├── maze_map_to_run.jpg
│   ├── objective_agent_path/
│       ├── objective_1_checkpoints.jpg
│       ├── objective_2_coverage.jpg
│
└── results/
    ├── policy/
    │   ├── policy1_checkpoints.csv
    │   ├── policy2_coverage.csv
    │
    ├── reward_formula/
        ├── reward1_checkpoints.json
        ├── reward2_coverage.json


```

---

# Future Improvements

Potential future work includes:

- Automated reward tuning
- Hyperparameter optimization
- Curriculum learning
- Multi-objective reward optimization
- Transfer learning to real robotic platforms

---

# Acknowledgements

Developed during **CSE SummerSchool 2026**.

We sincerely thank the organizers for providing the simulation platform and competition environment.

---

# License

This repository documents the engineering methodology and project outcomes only.

The simulator, datasets, and competition platform remain the intellectual property of the hackathon organizers.

Status: Completed as part of CSE SummerSchool Robotics Hackathon 2026.
