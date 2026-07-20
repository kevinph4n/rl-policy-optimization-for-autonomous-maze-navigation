# RL Policy Optimization for Autonomous Maze Navigation

A Reinforcement Learning (RL) policy optimization project developed during a robotics hackathon, focusing on autonomous robot navigation in a simulated maze environment.

The simulation platform and environment were provided by the organizers. Our work focused on improving the agent's navigation policy through reward engineering, iterative experimentation, and performance evaluation.

---

## Team

| Member | Contribution |
|---------|--------------|
| Phan Hong Phuc (me) | Reward engineering, policy optimization, experiment design, presentation - Objective 2 (Coverage) |
| Nguyen Chi Nguyen | Reward engineering, policy optimization, experiment design, presentation - Objective 1 Checkpoints) |
| Dao Cong Tri Bao | Reward engineering, policy optimization, experiment design, presentation - Objective 2 (Coverage) |
| Tran Hoang Son | Reward engineering, policy optimization, experiment design, presentation - Objective 3 (Wall-touching) |
| Nguyen Hoang Khang Huy | Reward engineering, policy optimization, experiment design, presentation - Objective 3 (Wall-touching) |

---

## Project Overview

### Objective

Develop an RL policy capable of navigating an autonomous robot through randomly generated maze environments while maximizing navigation performance.

The agent should learn to:

- Reach the goal efficiently
- Avoid collisions
- Minimize unnecessary movements
- Balance exploration and exploitation

---

## Environment

The simulator was provided exclusively by the hackathon organizers.

Features included:

- Randomly generated maze maps
- Robot agent
- Obstacles and walls
- Goal location
- Checkpoints
- Reward-based Reinforcement Learning framework

> **Note**
>
> Since the simulator is proprietary, its source code cannot be shared publicly.
> This repository documents our engineering process, methodology, and experimental findings.

---

## Individual Contribution (Phan Hong Phuc)

The primary engineering tasks included:

- Designing and refining the reward function
- Policy optimization through iterative experimentation
- Evaluating policy performance across 500+ generated maps
- Analyzing agent behaviors and navigation efficiency
- Preparing technical presentation slides
- Presenting experimental results

---

## Reward Policy

Example reward configuration:

| Event | Reward |
|--------|-------:|
| Reach Goal | +400 |
| Reach Checkpoint | +100 |
| Collision | -200 |
| Every Action | -2 |

The reward values were iteratively adjusted to improve:

- Navigation efficiency
- Collision avoidance
- Policy stability
- Exploration strategy

---

## Experiments

Multiple reward configurations were iteratively evaluated before selecting the final policy used during inference based on:
- Success rate
- Average path length
- Collision frequency
- Navigation stability
- Policy consistency

Evaluation was performed on more than **500 generated maze maps**.

---

## Results

The final policy demonstrated:

- Stable navigation across 500+ generated maps
- Effective collision avoidance
- Consistent goal-reaching behaviour
- Improved balance between exploration and exploitation

---

## Repository Structure

```
.
├── README.md
├── docs/
│   ├── Final_Slides.pdf
│   ├── Technical_Report.pdf
│   └── Architecture.png
│
├── images/
│   ├── maze_example.png
│   ├── navigation_result.gif
│   ├── reward_curve.png
│   └── inference.png
│
├── results/
│   ├── evaluation.md
│   └── experiments.md
│
└── videos/
    └── demo.mp4
```

---

## Gallery

### Maze Environment

*(Insert screenshot)*

---

### Navigation Result

*(Insert GIF or video)*

---

### Policy Performance

*(Insert charts or evaluation images)*

---

## Lessons Learned

This project strengthened our understanding of:

- Reinforcement Learning
- Reward Engineering
- Policy Optimization
- Autonomous Navigation
- Experimental Design
- Team Collaboration
- Engineering Communication

---

## Tech Stack

- Python
- Reinforcement Learning
- Autonomous Navigation
- Reward Engineering

*(Simulator provided by organizers)*

---

## Acknowledgements

This project was developed during **[Hackathon Name]** under the guidance of our mentor.

We sincerely thank the organizers for providing the simulation platform and competition environment.

---

## License

This repository documents the engineering methodology and project outcomes only.

The simulator, datasets, and competition platform remain the intellectual property of the hackathon organizers.
