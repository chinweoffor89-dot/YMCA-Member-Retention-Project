# 🏋️ YMCA Hold Likelihood Analysis  
### Data-Driven Insights for Proactive Member Retention  
**Role:** Team Lead & Lead Data Scientist  
**Project Type:** Academic–Industry Client Project  
**Client:** YMCA of Northern Alberta (Data Confidential)

---

## 📌 Project Overview

This project explores **membership hold behavior** at the YMCA to help identify members who are more likely to place their memberships on hold again.  
Rather than reacting after members disengage, the goal is to **anticipate hold likelihood** and enable **early, supportive intervention**.

⚠️ **Important Note:**  
Due to confidentiality agreements, **no raw data, model code, or notebooks are included** in this repository.  
This GitHub repository serves as a **visual, conceptual, and analytical showcase** of the work completed.

---

## 🎯 Problem Statement

Membership holds often precede long-term disengagement or cancellation.  
The YMCA wanted to understand:

- What behavioral patterns exist among members who go on hold?
- Can we segment members into **low, medium, and high likelihood** of going on hold again?
- How can these insights support proactive retention strategies?

---

## 💡 Business Value

The analysis enables the YMCA to:

- **Proactively engage** members before disengagement
- **Tailor communication strategies** based on likelihood segments
- **Optimize staff effort** by focusing outreach where it matters most
- Support member wellness while protecting long-term membership stability

---

## 🧠 Analytical Approach

### 1️⃣ Exploratory Data Analysis (EDA)
- Identified behavioral trends in hold frequency and duration
- Highlighted missing data patterns (e.g., age)
- Removed COVID-related holds after client feedback (pandemic outlier)

### 2️⃣ Feature Engineering
Key engineered features included:
- Hold duration
- Hold frequency (capped)
- Time between holds
- Member tenure
- Age and age group

These features helped capture **behavioral consistency and disengagement signals**.

---

## 3️⃣ Clustering for Explainable Segmentation

To avoid black-box labeling and ensure transparency:

- **K-Means Clustering (k=3)** was used to group members
- **PCA (Principal Component Analysis)** was applied to interpret clusters
- Behavioral patterns were reviewed and validated manually

### Cluster Interpretation:
| Segment | Description |
|------|-------------|
| Low Likelihood | Short, stable holds; consistent engagement |
| Medium Likelihood | Frequent but brief holds; moderate variability |
| High Likelihood | Long holds, quick returns to hold; early disengagement |

This process produced the final **hold_likelihood** target variable.

---

## 4️⃣ Predictive Modeling

Multiple supervised models were evaluated:

- Logistic Regression (baseline)
- Random Forest
- XGBoost
- Naïve Bayes
- **CatBoost (Selected Final Model)**

### Why CatBoost?
- Handles categorical variables natively
- Performs well on structured membership data
- Balanced performance across likelihood segments

**Key Metrics:**
- Accuracy ≈ 0.67
- F1-score prioritized over raw accuracy
- Conservative classification aligned with YMCA’s non-profit values

---

## 📊 Visualization & Communication

### Power BI Dashboard
A stakeholder-facing dashboard was built to visualize:
- Member demographics
- Hold behavior trends
- Segment distributions
- Location and tenure patterns

> Predictions were intentionally excluded per instructional guidance.

### Streamlit Prototype
An interactive prototype was developed to:
- Demonstrate segmentation logic
- Allow CSV uploads
- Present EDA and model outputs in a simplified UI

---

## 👩‍💼 Leadership & Collaboration

**Role: Team Lead (Epoch4)**  
- Coordinated a HyFlex team across virtual and in-person settings
- Led client communication and feedback integration
- Assigned tasks and managed deadlines via Microsoft Teams
- Led model development and deployment prototyping
- Translated technical findings into stakeholder-ready insights

---

## 🔁 Client Feedback Integration

Key client feedback directly shaped the project:
- Removed COVID-related data as a major outlier
- Reframed “risk” as **“likelihood”** to align with YMCA values
- Ensured clustering logic was transparent and explainable

---

## 🔮 Future Improvements

- Incorporate attendance and engagement data (check-ins, classes)
- Add time-series modeling for hold prediction windows
- Implement model monitoring and drift detection
- Deploy a secure internal dashboard for operational use

---

## 🚫 Data & Code Availability

Due to privacy and contractual constraints:
- ❌ No raw data included
- ❌ No notebooks or model files included
- ✅ Visual outputs and documented insights only

This repository is intended for **portfolio and knowledge demonstration purposes**.

---

## 📬 Contact

**Anthonia Offor**  
Team Lead & Data Scientist  
📍 Edmonton, Canada  
🔗 LinkedIn: *[www.linkedin.com/in/anthoniaoffor]*

