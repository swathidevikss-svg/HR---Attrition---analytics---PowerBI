1. Executive Summary & Business Impact
   
Overall Metrics: Analyzed 1,789 total employees (1,192 Active Headcount, 597 Historical Exits) with an overall Attrition Rate of 33.37%.
Financial Risk: Identified an estimated replacement cost exposure of ₹67 Million.
Interactive What-If Scenario: Implemented a parametric DAX model demonstrating that a 10% reduction in attrition saves ₹6.7 Million and retains 60 critical personnel.

2. Analytical Findings Across Report Views
   
Demographics & Work Mode: In-office staff had the highest attrition share (44.05%), while remote had only 18.93%. Commute times exceeding 45 minutes represented nearly 39% of departures. Peak departure tenure was in the 1–3 years (36.68%) and 3–5 years (28.64%) brackets.

Performance & Regrettable Loss: Out of 597 departures, 226 were Regrettable Exits (high performers/critical roles). Employee Net Promoter Score (eNPS) dropped from -3 (active) to -55 among leavers. Over 79% had received zero promotions.

Rewards & Compensation: 56.95% of departing staff had below-market compa-ratios, and 40.54% had not received a salary increment in 13–18 months.

AI Key Influencers: Machine learning driver analysis identified that being Below Market in Compa-ratio increases turnover probability by 3.00x, earning under ₹50K increases risk by 2.30x, and raise delays increase risk by 2.13x.

3. Data Architecture & Modeling
   
Data Model: Star Schema with a centralized `Master data` fact table connected via 1-to-many relationships to dimension tables (`DimDate`, `DimGrade`, `DimLocation`)
ETL Pipeline: Power Query transformation steps for type casting, handling missing values, and binning continuous variables (tenure bins, commute bands, compa-ratio tiers)
What-If Analysis: Disconnected parameter table (`Attrition Reduction %`) tied to dynamic DAX measures to calculate real-time savings scenarios for HR leadership.
Predictive Layer: Native Key Influencers visual leveraging embedded logistic regression algorithms.

