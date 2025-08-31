🚦 Road Traffic Collision Severity Analysis (UK, 2019–2023)
📌 Overview

This project analyses official UK Department for Transport (DfT) Road Safety Data (2019–2023) to assess how light (day vs. dark) and road surface conditions (dry vs. wet/adverse) influence the probability of a collision resulting in Killed or Seriously Injured (KSI) casualties.

📊 Data

Source: UK DfT Road Safety Data

Period: 2019–2023 (last-5-year + provisional 2024 combined)

Key variables: Accident_Index, Date, Light_Conditions, Road_Surface_Conditions, Casualty_Severity, Speed_Limit, Urban_or_Rural_Area, Local_Authority_District (LAD)

Outcome variable: KSI per accident. Derived flags:

is_dark = 1 if collision in darkness

is_wet = 1 if surface not dry

⚙️ Methods

Descriptive statistics – Monthly KSI per 100 collisions (2019–2023).

Relative Risk (RR) – Dark vs Day, Wet vs Dry (95% CI), stratified by speed & urban/rural.

Panel regression (Two-Way FE GLM) – LAD–month panel, binomial family, clustered SEs.

DST event study – Pre/post spring clock-change comparison.

🔑 Key Findings

Darkness dominates: KSI risk rises from 23/100 (day) to 41/100 (unlit dark). RR≈1.20.

Wetness weaker: RR≈1.08 overall, insignificant in many contexts.

Contextual effects: Strongest on urban 30–45 mph roads; urban RR≈1.24 vs rural RR≈1.18.

Temporal trends: U-shaped daily cycle; year-on-year upward drift.

DST shift: +1.95% post-spring clock change.

⚠️ Limitations

Reliance on police reports → possible under-reporting of slight injuries.

COVID-19 disrupted traffic patterns (esp. 2020).

🎯 Contributions & Policy Implications

Confirms global findings on visibility & weather with UK data.

Adds multidimensional analysis: speed, urbanisation, time, DST.

Policy priorities
Confirms global findings on visibility & weather with UK data.

Adds multidimensional analysis: speed, urbanisation, time, DST.

Policy priorities:

Improve night-time lighting & signage.

Strengthen high-speed & rural road safety.
Heighten vigilance during DST transitions.

👩‍🎓 Author: 刘增琦
📚 Course: CASA0006 — Quantitative Methods (UCL)
📅 Period: 2019–2023 UK DfT Road Safety Data

Improve night-time lighting & signage.

Strengthen high-speed & rural road safety.

Heighten vigilance during DST transitions.
