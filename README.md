# 基于分红障碍策略的跳跃扩散模型中欧洲期权定价的蒙特卡罗模拟(Application of Monte Carlo Simulation in Option  Pricing under a Geometric Brownian Motion with  Dividend Barrier Strategy)
# 项目简介

## 研究背景

在数学金融领域，许多文献探讨了为提供股息的基础资产定价的复杂性。本研究旨在使用蒙特卡罗模拟方法，在考虑股息障碍策略和风险中性概率测度的情况下，估算欧洲期权价格。

## 研究假设

- 假设基础股票在时间区间 [0, t] 内不支付股息，其累计对数回报率遵循几何布朗运动。
- 股息障碍策略会在基础资产价格超过股息障碍时触发即时股息支付。

## 研究方法

- 使用蒙特卡罗方法近似欧洲期权价格，通过**大数法则**将积分替换为样本均值。
- 通过带有常数边界“b”的欧拉离散化，在**Python**中模拟欧洲期权价格。
- 模拟结果与包含股息障碍策略（即Black-Scholes解法）的期权定价公式进行比较。

## 研究结论

- 结果显示，两种解法之间具有良好的收敛性。
- 值得注意的是，误差收敛率与问题的维度无关，使得该方法非常适合于高维期权定价以及涉及路径依赖型奇异期权和多资产期权模型的场景。

