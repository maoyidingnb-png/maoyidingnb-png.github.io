---
permalink: /experience/
title: "Experience"
author_profile: false
---

<style>
  .xp-section { margin-top:2em; }
  .xp-section h2 { border-bottom:1px solid #e5e7eb; padding-bottom:.3em; }
  .xp-item { border-left:3px solid #4b6fa8; padding:.1em 0 .1em 1em; margin:1.4em 0; }
  .xp-head { display:flex; flex-wrap:wrap; justify-content:space-between; align-items:baseline; gap:.2em 1em; }
  .xp-title { font-weight:700; font-size:1.05em; }
  .xp-date { color:#6b7280; font-size:.9em; white-space:nowrap; }
  .xp-sub { font-style:italic; color:#374151; font-size:.95em; margin:.15em 0 .4em; }
  .xp-item ul { margin:.3em 0 0 1.1em; }
  .xp-item li { font-size:.93em; margin:.3em 0; }
</style>

<div class="xp-section">
<h2>Research &amp; Projects</h2>

<div class="xp-item">
  <div class="xp-head"><span class="xp-title">World Model for Autonomous Systems</span><span class="xp-date">Jun 2026 – Present · Ningbo, China</span></div>
  <div class="xp-sub">Supervised by Dr. Huan Jin, AIOP Research Group</div>
  <ul>
    <li>Reproduced a Conditional Diffusion Transformer (CDiT)-based Navigation World Model for autoregressive prediction of future visual observations, conditioned on historical observations and actions.</li>
    <li>Deployed the NoMaD (Goal Masked Diffusion Policy) model with dynamic loss scaling to resolve the imbalance between action and distance losses, and designed an early-stopping mechanism based on the cosine similarity of trajectory direction, reaching 0.95+.</li>
    <li>Performed real-world data acquisition, obtaining relative position coordinates and trajectory yaw angles as spatiotemporal pose labels, and converted an 80 GB raw video stream into 20,000+ frames.</li>
    <li>Ran a controlled ablation across training duration (5-epoch vs. 10-epoch runs, 15 checkpoints in total): longer training raised trajectory-direction cosine similarity from about 0.94 to 0.97+ while substantially reducing both goal-conditioned distance loss and undirected action loss; with independent random initialisations, checkpoints at the same epoch across separate runs converged to distinct local optima rather than following comparable trajectories.</li>
  </ul>
</div>

<div class="xp-item">
  <div class="xp-head"><span class="xp-title">Deep Reinforcement Learning for Instant-Retail Supply-Chain Disruption</span><span class="xp-date">Dec 2025 – Present · Ningbo, China</span></div>
  <div class="xp-sub">Supervised by Dr. Ruijing Wu · <a href="https://github.com/maoyidingnb-png/rl_supply_chain">Code</a></div>
  <ul>
    <li>Built a discrete-event simulation environment in Python with a 94-dimensional MDP state space and 18 discrete actions, simulating supply-chain disruptions across one central warehouse, ten forward warehouses and five products.</li>
    <li>Implemented and compared DQN, DDQN, Dueling DQN, D3QN and PPO under a risk-enhanced initial-state distribution, increasing exposure to severe disruption scenarios within a constrained training budget.</li>
    <li>Applied Min-Max and standard normalisation for state preprocessing, implemented action masking to suppress invalid expediting actions during complete transportation failures, and used Common Random Numbers to reduce evaluation noise from Poisson demand and stochastic lead times.</li>
    <li>Evaluated learned policies against four non-RL baselines across ten disruption scenarios: D3QN, Dueling DQN and PPO matched the strongest heuristic in profit, outperformed aggressive hedging by 5.5%, and eliminated unnecessary expediting.</li>
  </ul>
</div>

<div class="xp-item">
  <div class="xp-head"><span class="xp-title">Mechanical Ventilation Modelling with ODEs</span><span class="xp-date">Jul 2025 – Aug 2025 · Ningbo, China</span></div>
  <div class="xp-sub">Supervised by Dr. Mainul Haque</div>
  <ul>
    <li>Developed ordinary differential equation models capturing the dynamics of airway pressure, intrinsic PEEP and arterial blood gas levels, with parameter optimisation.</li>
    <li>Implemented numerical simulations and visualisations in Python (NumPy) and MATLAB, replicating and validating published findings on the effect of PEEP on lung function in chronic airflow obstruction.</li>
    <li>Simulated airway pressure variation and gas-exchange efficiency under different PEEP settings.</li>
  </ul>
</div>
</div>

<div class="xp-section">
<h2>Industry</h2>

<div class="xp-item">
  <div class="xp-head"><span class="xp-title">Zhejiang Humanoid Robot Co., Ltd.</span><span class="xp-date">Jun 2026 – Sep 2026 · Ningbo, China</span></div>
  <div class="xp-sub">Platform Software Intern</div>
  <ul>
    <li>Analysed and validated the company's robot data platform across Apache Pulsar, IoTDB, Doris, MySQL and Kubernetes, tracing multi-source telemetry from real-time ingestion and messaging to time-series storage and analytical querying across 10+ telemetry and event streams.</li>
    <li>Built data-quality validation workflows that reconciled timestamps and cross-source identifiers and detected missing, duplicated and inconsistent telemetry, achieving 95%+ cross-source record-matching coverage for downstream analytics and debugging.</li>
    <li>Developed an enterprise AI code-review system based on Alibaba Open-Code-Review, integrating Git/CI, static analysis, repository-level retrieval and LLM agents; evaluated on 200+ labelled defects, it reached about 31.9% precision, 20.4% recall and 0.18 F1.</li>
    <li>Optimised diff-aware context retrieval and LLM review workflows, increasing true-positive defect detection by 7.7% on representative code changes.</li>
  </ul>
</div>

<div class="xp-item">
  <div class="xp-head"><span class="xp-title">BOE Technology Group Co.</span><span class="xp-date">Jun 2025 – Aug 2025 · Beijing, China</span></div>
  <div class="xp-sub">Data Analyst Intern</div>
  <ul>
    <li>Developed an employee-attrition analytics framework using 50,000+ records from 2022–2025, integrating personnel, factory, operational and external benchmark data to support workforce-risk planning.</li>
    <li>Cleaned and standardised multi-source records, handled missing and anomalous values, and engineered 20+ employee- and department-level features, including overtime intensity, compensation deviation, tenure and historical turnover.</li>
    <li>Built and compared linear regression, logistic regression and decision-tree models for department-level turnover forecasting and individual attrition prediction, reaching 0.84 AUC and 78% recall with the best classifier.</li>
    <li>Translated model outputs into Power BI dashboards and presented key attrition drivers and retention recommendations to departmental stakeholders.</li>
  </ul>
</div>

<div class="xp-item">
  <div class="xp-head"><span class="xp-title">Donghai Insurance</span><span class="xp-date">Jul 2024 – Aug 2024 · Ningbo, China</span></div>
  <div class="xp-sub">Data Analyst Intern</div>
  <ul>
    <li>Built a Python preprocessing workflow to clean and structure 20,000+ policy and claims records, constructing policyholder- and policy-level features for pricing analysis.</li>
    <li>Decomposed expected loss into frequency and severity: Poisson regression with a log-exposure offset for annualised claim frequency, and a log-normal model on log-transformed claim amounts for severity, using 15+ features; decision trees served as a benchmark and surfaced candidate interactions.</li>
    <li>Combined predicted frequency and severity to estimate expected loss and compare loss ratios across risk segments, supporting tiered coverage and premium-pricing recommendations.</li>
    <li>Validated model stability with 5-fold cross-validation and used feature importance to identify dominant risk factors, translated into risk-tier and premium-rating recommendations.</li>
  </ul>
</div>
</div>
