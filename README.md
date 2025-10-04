# A Network-Based Explanation of Stock Returns Using Minimum Spanning Tree (MST)

## Author

**Wang Lei** ([@wlxhfzh](https://github.com/wlxhfzh))

This repository documents my ongoing Master's Thesis research, which explores the intersection of network science and quantitative asset pricing. As an aspiring PhD candidate, my objective is to develop and empirically validate novel, data-driven frameworks for understanding the complex dynamics of financial markets.

---

## 1. Project Overview

Traditional asset pricing models, such as the CAPM and Fama-French multi-factor models, have provided a foundational paradigm for explaining stock returns through systematic risk factors. However, these linear models may not fully capture the complex, non-linear interactions and the hierarchical structure inherent in modern financial markets.

This research proposes an alternative framework to explain stock returns by leveraging network theory, specifically the **Minimum Spanning Tree (MST)**. The core hypothesis is that a stock's position and influence within the market's topological structure contain significant information about its future returns, beyond what is explained by conventional factors.

The central research question is: **Can topological metrics derived from the MST network of the China A-share market provide significant and unique explanatory power for cross-sectional stock returns?**

To address this, the project involves:
1.  Constructing dynamic correlation matrices from the daily returns of China A-share constituents.
2.  Filtering these dense matrices to generate a series of MSTs, which represent the core network backbone of the market.
3.  Extracting various node-level topological metrics from the MSTs (e.g., degree centrality, betweenness, eccentricity).
4.  Empirically testing the relationship between these network-derived metrics and subsequent stock returns through panel regressions and portfolio analysis.

This study aims to contribute a new, network-based perspective to the asset pricing literature, with a particular focus on the unique dynamics of the China A-share market.

---

## 2. Code Structure

The repository is organized into several modules, each corresponding to a key stage of the research workflow:

- **`/data_acquisition`**: Contains scripts for the automated collection and updating of historical market data for China A-shares, such as daily closing prices, trading volumes, and risk-free rates.

- **`/mst_construction`**: This module contains the core logic for building the network. It includes scripts for:
    1.  Calculating dynamic correlation matrices from stock return time series.
    2.  Transforming correlation matrices into distance matrices.
    3.  Applying algorithms (e.g., Kruskal's or Prim's) to generate the Minimum Spanning Tree.

- **`/empirical_analysis`**: This module contains the core econometric and statistical analysis of the project. It aims to test the explanatory power of the network-derived metrics. The scripts in this section perform the following tasks:
    1.  **Network Metrics Calculation**: Functions to compute various node-level topological metrics (e.g., Degree Centrality, Betweenness Centrality, Closeness Centrality) from the generated MSTs.
    2.  **Econometric Testing**: Scripts to run panel regressions (e.g., Fama-MacBeth) to test whether the network metrics can explain the cross-section of stock returns after controlling for traditional factors (e.g., Size, Value, Momentum).
    3.  **Portfolio Analysis**: Code to perform portfolio sorts based on the network metrics and analyze the performance (e.g., alpha, Sharpe ratio) of the resulting portfolios.

---

## 3. Important Notes on Availability

1.  **Code Access**: For reasons of data privacy and to maintain the integrity of the ongoing research, some portions of the source code have been omitted from this public repository. I am happy to provide the complete, functional code for academic review or collaboration purposes. Please contact me via email to request access.

2.  **Research Results**: The project is under active development. If you are interested in viewing the current research findings, visualizations, or a demonstration of the code's output, please feel free to send me an email.

---

## 4. Contact

I welcome any discussion, feedback, or collaboration opportunities related to this research.

- **Email**: `[2823115764@qq.com]`

