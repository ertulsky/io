---
layout: post
title:  "Convex Optimization LP and ML Rankings for Fantasy Football"
date:   2025-06-08T14:25:52-05:00
author: Evan Tulsky
categories: Projects
tags: Sports Analytics
permalink: /posts/fantasyfootball/
---

## Introduction

This project combines **machine learning** and **convex optimization** to help make smarter fantasy football draft decisions. The model forecasts player performance for the upcoming season and uses those predictions in a dynamic draft simulation with a **linear program (LP)** to optimize roster construction. Future projections will utilize a **Monte Carlo simulation**.

---

## Machine Learning Player Projections

I trained PyTorch-based regression models on player statistics from the 2024 season to **predict individual performance stats** (passing yards, rushing touchdowns, receptions, etc.) for 2025. Fantasy points are calculated by applying a standard half-PPR scoring system:

python
scoring = {
    'PassYds': 0.04,  # 1 pt per 25 yds
    'PassTD': 4,
    'Int': -2,
    'RushYds': 0.1,
    'RushTD': 6,
    'Rec': 0.5,
    'RecYds': 0.1,
    'RecTD': 6,
    'FL': -2
}

Using this rule-based mapping, we convert predicted stats into fantasy scores, rank the players, and generate projections for each position (QB, RB, WR, TE).

Feature Selection and Loss
The model uses standardized features like yards, touchdowns, fumbles, and receptions, and trains with mean squared error (MSE) loss. Epoch loss is tracked to ensure convergence:
Epoch 0, Loss: 16259.50
...
Epoch 300, Loss: 25.67

We also visualize feature importance using model weights to interpret which inputs most affect the predictions.

## Convex Optimization for Team Building
Once projections are finalized, we solve a convex optimization problem to build the optimal fantasy team under roster constraints. The LP selects a lineup maximizing total projected fantasy points while satisfying positional requirements (e.g., 2 RBs, 3 WRs, 1 TE, etc.).

The LP is solved using cvxpy, and the optimal draft choices are compared to the Monte Carlo output to plan future picks.

objective = cp.Maximize(cp.sum(selected_players["FantasyScore"]))
constraints = [
    total_players == 9,
    num_RBs >= 2,
    num_WRs >= 3,
    num_TEs == 1,
    ...
]
prob = cp.Problem(objective, constraints)
prob.solve()

Optimized Roster from CVX Solver:
QB: Lamar Jackson
RB: Tony Pollard, Rico Dowdle
WR: A.J. Brown, Malik Nabers
TE: George Kittle
Flex: Joe Mixon
Total Projected: 1430.5 pts


