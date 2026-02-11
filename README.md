# H1N1 Vaccine Prediction Project

### **Stakeholder: Department of Public Health (DPH)**

---

## Project Overview
In the wake of the 2009 H1N1 pandemic, public health organizations faced the monumental task of predicting and encouraging vaccine uptake. This project utilizes data from the **National 2009 H1N1 Flu Survey** to build a predictive model that identifies whether an individual received the H1N1 vaccine. 

By analyzing behavioral patterns, personal opinions, and demographic backgrounds, we provide a data-driven framework for future public health interventions.

---

## Business Problem
The primary challenge for public health stakeholders is **vaccine hesitancy and inefficient resource distribution**. During an outbreak, time and medical resources are limited. This project identifies key drivers of uptake to help the DPH target educational campaigns and mobile clinics effectively.

* **Primary Metric:** ROC-AUC Score (Target: ≥ 0.80)
* **Business Priority:** High Recall (to minimize missed opportunities for outreach)

---

## Methodology & Modeling
This project followed an iterative statistical modeling process to ensure both interpretability and predictive power:

1.  **Baseline Logistic Regression:** Provided a statistical foundation to quantify the impact of specific factors.
2.  **Decision Trees:** Captured non-linear relationships and visualized complex decision paths.
3.  **Tuned Random Forest (Final Model):** Achieved optimal performance through hyperparameter tuning and threshold optimization.



---

## Key Findings & Model Performance
The model was refined to balance overall accuracy with the specific needs of public health outreach.

* **Final ROC-AUC:** **0.8289** (Successfully surpassed the 0.80 target).
* **Optimized Recall:** By shifting the decision threshold to **0.3**, we achieved a **Macro Average Recall of 0.75**.
* **Top Predictors:** * **Doctor Recommendations:** The single most significant driver of vaccination (`doctor_recc_h1n1`).
    * **Perceived Risk & Effectiveness:** These psychological factors showed higher predictive power than actual knowledge levels.



---

## Actionable Recommendations
Based on the model insights, we recommend the following strategies for the DPH:

1.  **Physician-Led Campaigns:** Partner with medical clinics to ensure providers are actively recommending the vaccine during routine visits.
2.  **Safety-First Messaging:** Pivot outreach to focus specifically on the **safety and effectiveness** of the vaccine to address perceived risks.
3.  **Behavioral Targeting:** Focus resources on individuals who regularly receive the seasonal flu vaccine, as they are the most likely to accept the H1N1 vaccine.

---

## Conclusion
The **Tuned Random Forest model** allows the DPH to transition from broad outreach to targeted, evidence-based interventions. By optimizing for **Recall**, we ensure that limited resources are directed toward the specific drivers that increase community immunity and save lives.

---

### Repository Structure
* `notebook.ipynb`: Full data cleaning, EDA, and modeling process.
* `data/`: Directory containing the survey datasets.
* `README.md`: Project summary and findings.

### Author
**Abdullahi Abdi Hassan** *BSc Statistics Graduate | Data Science Student at Moringa School*
