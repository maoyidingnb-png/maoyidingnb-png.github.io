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
    <li>Curated a 20,000+ frame dataset from 80 GB of self-collected real-world navigation video, labeled with spatio-temporal poses derived from relative positions and trajectory yaw angles.</li>
    <li>Trained and optimized NoMaD (Goal Masked Diffusion Policy) with dynamic loss scaling to balance the action and distance objectives, and designed an early-stopping criterion based on trajectory-direction cosine similarity to select checkpoints across extended training runs (5 vs. 10 epochs, 15 checkpoints), raising cosine similarity from approximately 0.94 to above 0.97 while reducing both goal-conditioned distance and undirected action losses.</li>
    <li>Reproduced the Conditional Diffusion Transformer (CDiT)-based Navigation World Model for autoregressive prediction of future visual observations from past observations and actions to enable model-based evaluation of candidate actions.</li>
    <li>Integrated the two models by employing the world model to score and rank NoMaD-sampled candidate trajectories offline, identifying the insufficiency of visual plausibility in validating world-model-based planning due to the possible deviation from ground-truth observations of subsets of predicted frames.</li>
  </ul>
</div>

<div class="xp-item">
  <div class="xp-head"><span class="xp-title">A Deep Reinforcement Learning-Based Strategy for Instant Retail Supply Chain Interruption</span><span class="xp-date">Dec 2025 – Present · Ningbo, China</span></div>
  <div class="xp-sub">Supervised by Dr. Ruijing Wu · <a href="https://github.com/maoyidingnb-png/rl_supply_chain">Code</a></div>
  <ul>
    <li>Formulated instant-retail disruption response as a Markov decision process (MDP), modeling supplier-capacity and transport disruptions as Markov-modulated states, encoding buffer level, expediting and allocation priority as 18 discrete actions with physically motivated masking, and defining an inventory position that includes capacity and transport backlogs to prevent duplicate ordering.</li>
    <li>Developed a reproducible training and evaluation pipeline for 25 agents (5 DRL algorithms × 5 seeds) over 2.25M simulated days, incorporating common random numbers, independent random-number streams for demand, disruptions and lead times, and risk-augmented initial states to improve coverage of rare, severe disruption states.</li>
    <li>Designed an evaluation protocol addressing seed sensitivity and pseudo-replication documented in DRL research, with the training seed as the statistical unit and paired confidence intervals, establishing that the base (s, S) policy outperformed all DRL agents, and attributing the gap to differences in their ordering behavior and post-disruption recovery.</li>
    <li>Developed a revised framework to address structural limitations of the benchmark formulation, introducing a lost-sales MDP to allow disruptions also delaying in-transit inventory, a masked autoregressive PPO policy generating joint integer purchase and shipment decisions, a proof to ensure the policy generates exactly the feasible action set, and an exact bounded-cost reformulation preserving policy rankings.</li>
  </ul>
</div>

<div class="xp-item">
  <div class="xp-head"><span class="xp-title">Clinical Mechanical Ventilation Modeling</span><span class="xp-date">Jul 2025 – Aug 2025 · Remote</span></div>
  <div class="xp-sub">Supervised by Dr. Mainul Haque</div>
  <ul>
    <li>Built an ODE model of mechanical ventilation capturing airway pressure, intrinsic PEEP and arterial blood-gas dynamics, and estimated its parameters by numerical optimization in Python (NumPy) and MATLAB.</li>
    <li>Simulated airway pressure and gas-exchange efficiency across PEEP settings and reproduced published findings on the effect of PEEP in chronic airflow obstruction, validating the model against the literature.</li>
  </ul>
</div>
</div>

<div class="xp-section">
<h2>Industry</h2>

<div class="xp-item">
  <div class="xp-head"><span class="xp-title">Zhejiang Humanoid Robot Co., Ltd.</span><span class="xp-date">Jun 2026 – Sep 2026 · Ningbo, China</span></div>
  <div class="xp-sub">Platform Software Intern</div>
  <ul>
    <li>Developed ROS 2 nodes to read robot telemetry and traced 10+ telemetry and event streams through the company’s data platform (Apache Pulsar, IoTDB, Doris and MySQL on Kubernetes), from real-time ingestion to time-series storage and analytical querying.</li>
    <li>Built data-quality validation workflows to reconcile timestamps and cross-source identifiers, and flag missing, duplicated, and inconsistent records, reaching 95%+ cross-source record matching for downstream analytics and debugging.</li>
    <li>Worked on the tour-guide, data-collection, and teleoperation apps on physical robots; diagnosed a relocalization-status display failure by tracing from the UI through ROS communication to robot-side topics, isolating the fault to the application layer, implementing the fix, and verifying it on the physical robot after release.</li>
    <li>Extended an LLM-based code-review system built on Alibaba Open-Code-Review with diff-aware context retrieval and a code knowledge graph, increasing true-positive defect detection by 7.7%; proposed a no-plan mode for rule-matched tasks, achieving a reduction in review time to ~1/7 and cost by ~50% on an internal sample.</li>
  </ul>
</div>

<div class="xp-item">
  <div class="xp-head"><span class="xp-title">BOE Technology Group Co.</span><span class="xp-date">Jun 2025 – Aug 2025 · Beijing, China</span></div>
  <div class="xp-sub">Data Analyst Intern</div>
  <ul>
    <li>Built an employee-attrition analytics framework on 50,000+ records from 2022–2025, integrating personnel, factory, operational and external benchmark data to support workforce-risk planning.</li>
    <li>Cleaned and standardized multi-source records, handled missing and anomalous values, and engineered 20+ employee- and department-level features, including overtime intensity, compensation deviation, tenure and historical turnover.</li>
    <li>Used linear regression for department-level turnover forecasting and compared logistic regression with decision-tree classifiers for individual attrition prediction; the best classifier reached 0.84 AUC and 78% recall.</li>
    <li>Identified the key predictors of attrition and translated them into Power BI dashboards and retention recommendations for departmental stakeholders.</li>
  </ul>
</div>

<div class="xp-item">
  <div class="xp-head"><span class="xp-title">Donghai Insurance</span><span class="xp-date">Jul 2024 – Aug 2024 · Ningbo, China</span></div>
  <div class="xp-sub">Data Analyst Intern</div>
  <ul>
    <li>Built a Python-based data preprocessing workflow to clean and structure 20,000+ policy and claims records, constructing policyholder- and policy-level features for pricing analysis.</li>
    <li>Developed frequency and severity models to decompose expected loss by implementing Poisson regression with a log-exposure offset to model annualized claim frequency, and a log-normal severity model fitted on log-transformed claim amounts over the claims-incurred subset with 15+ policyholder and policy features; decision trees were fitted as a benchmark and to surface candidate interactions.</li>
    <li>Combined predicted frequency and severity to estimate expected loss and compare loss ratios across risk segments; validated model stability with 5-fold cross-validation and used feature-importance analysis to identify the dominant risk factors.</li>
  </ul>
</div>
</div>
