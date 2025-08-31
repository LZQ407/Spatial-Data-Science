Road Traffic Collision Severity Analysis (UK, 2019–2023)
Overview

This project analyses official UK Department for Transport (DfT) Road Safety Data (2019–2023) to assess how light (day vs. dark) and road surface conditions (dry vs. wet/adverse) influence the probability of a collision resulting in Killed or Seriously Injured (KSI) casualties.

The study also examines how these effects vary across speed limits and urban–rural contexts, explores hourly and seasonal patterns, and evaluates the impact of the Daylight Saving Time (DST) transition.

Data

Source: UK DfT Road Safety Data

Period: 2019–2023 (last-5-year + provisional 2024 releases combined)

Key variables:

Accident_IndexAccident_Index (unique ID)

Date, Time

Light_ConditionsLight_Conditions, Road_Surface_ConditionsRoad_Surface_Conditions

Casualty_SeverityCasualty_Severity (fatal / serious / slight)

Speed_LimitSpeed_Limit, Urban_or_Rural_AreaUrban_or_Rural_Area

Local_Authority_District (LAD)

The primary outcome variable is KSI count per collision, with binary indicators:

is_dark = 1 if collision in darkness, 0 if daylight

is_wet = 1 if surface not dry, 0 if dry

Methods

Four analytical approaches were applied:

Descriptive statistics: monthly trends of KSI per 100 collisions.

Relative Risk (RR): comparing Dark vs Day, Wet vs Dry (with 95% CI), including stratified analysis by speed and urban/rural.

Panel regression (Two-Way Fixed Effects GLM):

LAD–month panel

Model:

ksi_rate
∼
share_dark
+
share_wet
+
𝐶
(
month
)
+
𝐶
(
LAD
)
ksi_rate∼share_dark+share_wet+C(month)+C(LAD)

Binomial family, clustered SEs.

Quasi-experiment (DST event study): pre/post comparison around spring DST shifts (2019–2023).

Key Findings

Darkness is the dominant risk factor:

KSI risk rises from ~23/100 collisions in daylight to ~41/100 in unlit dark.

RR ≈ 1.20 (20% higher risk in darkness).

Wet surfaces play a smaller role:

RR ≈ 1.08 overall, but effects are weak or inconsistent across contexts.

Contextual heterogeneity:

Dark effects strongest on urban mid-speed roads (30–45 mph).

Urban RR ≈ 1.24 vs rural RR ≈ 1.18.

Temporal patterns:

Clear U-shaped daily cycle (highest risk at night/early morning, lowest in morning peak).

Seasonal and year-on-year upward drift in severity.

DST effect:

Average +1.95% increase in severity after spring clock change, consistent with international evidence.

Limitations

Reliance on police-reported accidents (possible under-reporting of slight injuries).

COVID-19 pandemic may distort 2020 patterns.

Contributions & Policy Implications

Validates international findings on visibility and weather using UK data.

Adds a multidimensional perspective by incorporating speed, urbanisation, temporal patterns, and DST.

Suggests policy priorities:

Improve night-time lighting and signage.

Target high-speed and rural roads for safety interventions.

Consider preventive measures around DST transitions.
