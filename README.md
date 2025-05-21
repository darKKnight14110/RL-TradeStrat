# 🧠 Deep Q-Learning for Stock Trading  
> *“Markets are puzzles. Reinforcement learning is our scalpel.”*  
> — A Quant

---

## 🧬 Approach

This project uses a **Deep Q-Network (DQN)** to train a trading agent on the **Nifty 50 index**, which has exhibited high volatility and multiple trend reversals over the past 5 years — a perfect testbed for dynamic, policy-driven strategies.

### 🎯 Problem Setup

- **Dataset**: Daily closing prices of **Nifty 50** (last 5 years)
- **State**: Sequence of `n` price differences, sigmoid-normalized
- **Actions**:  
  `0`: Hold  
  `1`: Buy  
  `2`: Sell  
- **Reward**: Realized profit per transaction (net of fees)
- **Constraints**:  
  • **Transaction fee** of `0.15%` per trade  
  • **Forced liquidation** at episode end  
  • Experience replay + ε-greedy policy

### 🧠 Model Architecture

```
Input Layer (n features)
↓
Dense (64) — ReLU  
↓  
Dense (32) — ReLU  
↓  
Dense (8) — ReLU  
↓  
Output Layer (3 actions) — Linear  
```

---

## 📊 Results

Trained and evaluated on **volatile Nifty 50 data**, capturing both bull and bear swings, gap-downs, and false breakouts.

| Metric           | Value       |
|------------------|-------------|
| **Total Profit** | `Rs+157723.37`  |
| **Return**       | `+1.32%`     |

---

### 📉 Trade Plots

#### Nifty50 Close Price:
![image](https://github.com/user-attachments/assets/887a99dd-8c76-44f0-9b2b-2461a572dd86)

#### Sample trade plot on Episode 3:
![image](https://github.com/user-attachments/assets/6694ac1f-4128-4f11-8018-02b7c8664c05)

---
