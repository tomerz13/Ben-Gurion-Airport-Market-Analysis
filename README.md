# The Geopolitical Substitution Effect: Aviation Data Analysis in the Shadow of War ✈️🌍

## 1. Executive Summary
This project analyzes the structural shift in the Israeli aviation market following the outbreak of the "Iron Swords" war (October 2023). Using a comprehensive dataset of passenger traffic from Ben Gurion Airport (2022-2025), this end-to-end analytical research explores how consumers adapt to severe supply constraints and the de-facto geopolitical boycott of the Turkish aviation market. Designed from the perspective of an Aviation Data Analyst, the project utilizes **Python** to build a robust econometric Difference-in-Differences (DiD) model, complete with algorithmic control group selection and automated data visualization.

## 2. Business Problem

**The Context:** The aviation industry is highly sensitive to exogenous shocks. In October 2023, the Israeli aviation market faced an unprecedented crisis: a sharp drop in flight supply and a complete shutdown of its top destination—Turkey (Istanbul as a global Hub, and Antalya as a Leisure destination). 

**The Problem:** Without empirical evidence, airlines, tourism boards, and network planners struggle to predict where passenger demand will shift during prolonged geopolitical crises. Do passengers cancel flights entirely (inelastic demand), or do they immediately seek alternatives (destination switching)?

**The Objective:** This analytical project provides actionable insights for Aviation Strategists and Route Planners by answering three core questions:
1. **Hub Substitution:** Can Gulf carriers (UAE) successfully capture the transit traffic lost by Istanbul?
2. **Leisure Substitution:** Where does the short-haul Mediterranean vacation demand shift when a primary competitor is removed?
3. **Demand Elasticity:** Are long-haul, "essential" routes (e.g., USA) affected by regional geopolitical boycotts, or is their demand inelastic?

## 3. Methodology & Approach
To isolate the true "Substitution Effect" from the general market downturn caused by the war, a strict econometric framework was implemented:
* **Data Engineering:** Processed monthly panel data, filtering out statistical noise by removing marginal destinations (keeping only robust routes with >200,000 historical passengers).
* **Algorithmic Matching:** Developed a Python algorithm using Pearson Correlation and RMSE to objectively identify the optimal Control Groups (e.g., London Heathrow for the UAE, Varna for Greece/Cyprus) based on pre-war parallel trends.
* **Econometric Modeling (DiD):** Executed Ordinary Least Squares (OLS) regressions using the `statsmodels` library. The model controls for systemic seasonality (Month Fixed Effects) and isolates short-term security events (Pulse variables).

## 4. Skills & Tools
* **Languages:** Python (Pandas, NumPy, Matplotlib, Statsmodels)
* **Tools:** Jupyter Notebook / IDE, GitHub
* **Analytical Skills:** Econometrics (Difference-in-Differences, OLS), Time-Series Analysis, Control Group Matching, Causal Inference, Data Visualization, Aviation Economics.

## 5. Results & Business Recommendations
* **Aggressive Leisure Substitution:** The data reveals a massive **+7.6%** surge in market share for Greece & Cyprus. **Recommendation:** Mediterranean airlines and tourism boards should heavily target capacity expansion (slots) and localized marketing during regional crises, as leisure travelers exhibit extreme destination flexibility.
* **Hub Route Optimization:** The UAE successfully captured a **+2.2%** structural increase in market share, proving its status as a direct substitute for Istanbul. **Recommendation:** Gulf carriers should optimize dynamic pricing and expand transit flight frequencies when competing hubs face geopolitical friction.
* **Inelastic Long-Haul Markets:** A Placebo test on the US market (New York vs. LA) showed zero significant substitution effect. **Recommendation:** Network planners can rely on long-haul essential routes as stable revenue anchors during regional crises.

## 6. Visualization Preview

![Hub Substitution](link_to_your_graph_1_image.png)
*Figure 1: The structural break in Hub market share (UAE vs. London Heathrow) following the October 2023 shock.*

![Leisure Substitution](link_to_your_graph_2_image.png)
*Figure 2: The aggressive substitution effect in the Leisure market (Greece & Cyprus vs. Varna).*

---

**Data Note:** The raw panel data was compiled from the official public activity reports of the Israel Airports Authority (IAA). To comply with data ownership, only the analytical Python script and resulting visualizations are hosted in this repository.
