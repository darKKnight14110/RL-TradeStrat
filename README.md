# 🧠 Deep Reinforcement Learning for Trading & Portfolio Allocation

This repository combines two advanced reinforcement learning (RL) systems designed for algorithmic trading and dynamic portfolio allocation. Built using Deep Q-Learning, both projects aim to optimize investment strategies through data-driven, adaptive learning.

---

## 📊 1. Stock Trading Agent (Nifty50)

A Deep Q-Learning agent trained on the highly volatile **Nifty50** index over the past 5 years. The model learns optimal buy/sell/hold actions based on historical price movements, with real-world constraints like transaction fees incorporated.

### ⚙️ Key Highlights

- **Environment**: Historical daily price data from Nifty50
- **Actions**: Buy, Sell, Hold
- **Reward**: Realized profit minus 0.15% transaction costs per trade
- **Outcome**: A trained agent that learns to navigate noisy market environments and generate positive cumulative returns

### 💡 Impact

- Learns to exploit short-term price fluctuations.
- Generates trading strategies that outperform random and naive benchmarks.
- Provides visual insight into decision points with profit annotation.

### 📈 Sample Output

![WhatsApp Image 2025-05-21 at 17 10 07_9825703f](https://github.com/user-attachments/assets/c97c53ba-acad-499c-bf1b-b7cc18c46976)

---

## 💼 2. RL-Based Portfolio Allocation

A portfolio management framework using RL to dynamically rebalance investments across multiple cryptocurrencies. The agent is trained to optimize for **risk-adjusted returns** in a simulated trading environment.

### ⚙️ Key Highlights

- **Environment**: Cryptocurrency exchange data from Kaggle (2018)
- **State Representation**: Correlation matrix of asset returns
- **Reward Function**: Sharpe Ratio – balancing return and volatility
- **Actions**: Portfolio weight allocation and rebalancing

### 💡 Impact

- Achieves **higher returns**, **higher Sharpe ratio**, **lower volatility**, and **better alpha** compared to equal-weight and static benchmarks.
- Learns strategies that are **negatively correlated with the market**, enhancing diversification.
- Framework is flexible, extendable, and ideal for **robo-advisors** and **automated fund management**.

### 📊 Performance Summary

- 🚀 Higher cumulative returns vs baseline
- 📉 Reduced drawdowns during market turbulence
- 📈 Smarter rebalancing during volatile periods

### 🖼️ Portfolio Behavior Example

![image](https://github.com/user-attachments/assets/86860498-9e7f-4dcd-ae22-9dc466f40dbe)


---

## 🔍 Why This Matters

These systems are a step beyond traditional finance techniques:

- No manual rules — strategies are learned directly from data
- Adaptive to dynamic market environments
- Realistic with inclusion of trading costs and risk management

From timing single-stock trades to balancing portfolios across assets, this repository showcases how reinforcement learning can drive **next-generation investment systems**.
