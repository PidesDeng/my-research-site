---
title: "基于MCNP的中子输运模拟流程"
date: 2026-07-29
draft: false
tags: ["中子输运", "MCNP", "蒙特卡洛"]
categories: ["模拟计算"]
math: true
---

## 研究背景

本研究基于蒙特卡洛方法，对反应堆堆芯中子输运过程进行数值模拟分析。

## 核心方程

稳态中子输运方程如下：

$$
\Omega \cdot \nabla \psi(\vec{r}, E, \Omega) + \Sigma_t \psi = \int_0^\infty \int_{4\pi} \Sigma_s \psi \, d\Omega' dE' + S
$$

## 计算流程

1. 建立几何模型
2. 定义材料截面数据
3. 设置粒子源项
4. 运行MCNP计算
5. 提取通量分布结果
