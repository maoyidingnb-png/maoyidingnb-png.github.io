---
permalink: /
author_profile: false
redirect_from: 
  - /about/
  - /about.html
---

<style>
  .hp-header { display:flex; flex-wrap:wrap; align-items:center; gap:2em; margin:1em 0 2.2em; }
  .hp-photo { width:180px; height:auto; border-radius:10px; flex-shrink:0; box-shadow:0 2px 10px rgba(0,0,0,.12); }
  .hp-info { flex:1; min-width:240px; }
  .hp-info h1 { margin:0 0 .25em; font-size:2em; }
  .hp-info p { margin:.15em 0; }
  .hp-role { font-size:1.05em; }
  .hp-muted { color:#6b7280; font-size:.92em; }
  .hp-links { margin-top:.8em !important; font-size:.95em; }
  .hp-links a { margin-right:1.1em; text-decoration:none; }
  .hp-section { margin-top:2.2em; }
  .hp-section h2 { border-bottom:1px solid #e5e7eb; padding-bottom:.3em; }
  .hp-card { border-left:3px solid #4b6fa8; padding:.2em 0 .2em 1em; margin:1.2em 0; }
  .hp-card h3 { margin:0 0 .35em; font-size:1.05em; }
  .hp-card p { margin:.3em 0; font-size:.95em; }
  .hp-tags { margin-top:.4em; }
  .hp-tag { display:inline-block; font-size:.78em; padding:.12em .6em; margin:.15em .3em .15em 0; border-radius:999px; background:#eef2f8; color:#3b5583; }
  .hp-proj { margin:1em 0; }
  .hp-proj p { margin:.2em 0; font-size:.95em; }
  .hp-edu { list-style:none; margin-left:0; padding-left:0; }
  .hp-edu li { margin:.4em 0; }
  .hp-right { float:right; color:#6b7280; font-size:.9em; }
</style>

<div class="hp-header">
  <img class="hp-photo" src="/images/profile-portrait.jpg" alt="Yiding Mao">
  <div class="hp-info">
    <h1>Yiding Mao</h1>
    <p class="hp-role">BSc Statistics</p>
    <p class="hp-muted">University of Nottingham Ningbo China &amp; University of Nottingham</p>
    <p class="hp-links">
      <a href="mailto:smyym8@nottingham.ac.uk">Email</a>
      <a href="https://github.com/maoyidingnb-png">GitHub</a>
      <a href="/files/CV.pdf">CV</a>
    </p>
  </div>
</div>

<div class="hp-section" markdown="1">

## About Me

I am a Statistics undergraduate on the 2+2 programme at the University of Nottingham Ningbo China and the University of Nottingham, with a cumulative GPA of 3.98/4.00. My path into AI has run through progressively harder kinds of uncertainty: statistical models of insurance claims and employee attrition, reinforcement learning agents making sequential decisions under supply-chain disruption, and world models that learn how a robot's environment evolves from real video and sensor data.

Along the way, one question has kept returning: **a learned model can perform well and still be wrong in ways it cannot signal.** I want to understand how learned models of the world can quantify their own uncertainty, so that the systems relying on them know when to trust their predictions.

</div>

<div class="hp-section">

<h2>Research Interests</h2>

<div class="hp-card">
  <h3>World Models for Embodied AI</h3>
  <p>Learning predictive models of how the world responds to an agent's actions, directly from egocentric video and sensor data, and using them to plan. I have reproduced a CDiT-based navigation world model and trained the NoMaD diffusion policy on a campus dataset I collected and aligned myself.</p>
  <div class="hp-tags"><span class="hp-tag">world models</span><span class="hp-tag">diffusion models</span><span class="hp-tag">robot navigation</span></div>
</div>

<div class="hp-card">
  <h3>Reliability and Uncertainty of Learned Models</h3>
  <p>When can a learned model's predictions be trusted? Multi-step rollouts can look plausible while encoding incorrect future states, and identically configured runs can converge to distinct local optima. I am interested in principled ways to quantify these failures, rather than relying on heuristic training signals.</p>
  <div class="hp-tags"><span class="hp-tag">uncertainty quantification</span><span class="hp-tag">model evaluation</span><span class="hp-tag">trustworthy ML</span></div>
</div>

<div class="hp-card">
  <h3>Sequential Decision-Making under Uncertainty</h3>
  <p>Reinforcement learning in stochastic, disruption-prone environments, with careful experimental design. In a supply-chain study, Common Random Numbers, multi-seed training and heuristic baselines showed that policies with near-identical fill rates can operate a system in very different ways.</p>
  <div class="hp-tags"><span class="hp-tag">reinforcement learning</span><span class="hp-tag">MDPs</span><span class="hp-tag">experimental design</span></div>
</div>

</div>

<div class="hp-section" markdown="1">

## Selected Projects

<div class="hp-proj" markdown="1">
**World Model for Autonomous Systems** <span class="hp-right">Jun 2026 – Present</span>  
*Supervised by Dr. Huan Jin, AIOP Research Group*  
Built a spatiotemporally aligned dataset of 20,000+ frames from 80 GB of campus video; reproduced a CDiT navigation world model and trained NoMaD; an ablation over training length raised trajectory-direction cosine similarity from about 0.94 to 0.97+.
</div>

<div class="hp-proj" markdown="1">
**Deep RL for Instant-Retail Supply-Chain Disruption** <span class="hp-right">Dec 2025 – Present</span>  
*Supervised by Dr. Ruijing Wu* · [Code](https://github.com/maoyidingnb-png/rl_supply_chain)  
A discrete-event MDP with one central warehouse, ten forward warehouses and five products; D3QN, Dueling DQN and PPO matched the strongest heuristic in profit and outperformed aggressive hedging by 5.5%.
</div>

More details on the [Experience](/experience/) page.

</div>

<div class="hp-section" markdown="1">

## Education

<ul class="hp-edu">
  <li><strong>University of Nottingham</strong>, BSc Statistics <span class="hp-right">Sep 2025 – Present</span></li>
  <li><strong>University of Nottingham Ningbo China</strong>, BSc Statistics (2+2) <span class="hp-right">Sep 2023 – Present</span></li>
</ul>

</div>
