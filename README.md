1. Executive Summary & Business Impact
   
Overall Metrics: Analyzed 1,789 total employees (1,192 Active Headcount, 597 Historical Exits) with an overall Attrition Rate of 33.37%.
Financial Risk: Identified an estimated replacement cost exposure of ₹67 Million.
Interactive What-If Scenario: Implemented a parametric DAX model demonstrating that a 10% reduction in attrition saves ₹6.7 Million and retains 60 critical personnel.

2. Dataset Overview

The dataset contains various attributes related to employee demographics, work mode, compensation, and performnace. Key features include:
Employee ID
Department and Job Band/Grade 
Work Mode and Work Location 
Termination Type
Base Salary & variable bonus
Salary Group and Compa-Ratio Group 
Performance Score and Promotion History.  
Employee Net Promoter Score (eNPS)
Recognition Counts/Types.

3. Analytical Findings Across Report Views
   
Demographics & Work Mode: In-office staff had the highest attrition share 44.05%, while remote had only 18.93%. Commute times exceeding 45 minutes represented nearly 39% of departures. Peak departure tenure was in the 1–3 years 36.68% and 3–5 years 28.64% brackets.

Performance & Regrettable Loss: Out of 597 departures, 226 were Regrettable Exits (high performers/critical roles). Employee Net Promoter Score (eNPS) dropped from -3 (active) to -55 among leavers. Over 79% had received zero promotions.

Rewards & Compensation: 56.95% of departing staff had below-market compa-ratios, and 40.54% had not received a salary increment in 13–18 months.

AI Key Influencers: Machine learning driver analysis identified that being Below Market in Compa-ratio increases turnover probability by 3x, earning under ₹50K increases risk by 2.3x, and raise delays increase risk by 2.13x.

4. Strategic Recommendations
   
Correct Below-Market Pay:
Over 56% of departed staff were paid below market, which triples exit risk 3x. Prioritize immediate salary parity reviews for junior and mid-level bands in Engineering and HR to reduce early-career departures. 

Enforce Annual Appraisals:
Over 40% of exits waited 13–18 months for a pay raise (2.13x exit risk). Implement a strict 12-month increment review to prevent the major tenure drop-off occurring between years 1 and 3. 

Offer Flexible Work for Long Commutes:
On-site staff make up 44% of turnover, and commutes over 45 minutes account for nearly 39% of exits. Provide hybrid or remote options for employees with long commutes to cut travel-driven resignations.

Build Promotion and Recognition Paths:
Nearly 80% of exiting employees received zero promotions and 71% had no recognitions, driving leaver eNPS down to -55. Introduce transparent promotion tracks and spot rewards to protect the 226 high-performing, regrettable exits. 

5. Data Architecture & Modeling
   
Data Model: Star Schema with a centralized Master data fact table connected via 1-to-many relationships to dimension tables (DimDate, DimGrade, DimLocation)
ETL Pipeline: Power Query transformation steps for type casting, handling missing values, and binning continuous variables (tenure bins, commute bands, compa-ratio tiers)
What-If Analysis: Disconnected parameter table (Attrition Reduction %) tied to dynamic DAX measures to calculate real-time savings scenarios for HR leadership.
Predictive Layer: Native Key Influencers visual leveraging embedded logistic regression algorithms.



