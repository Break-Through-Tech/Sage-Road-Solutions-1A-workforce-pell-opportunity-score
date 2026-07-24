---

> ## Challenge Advisor: Update & Finalize Your Project Overview
>
> > 💡 **These grey text instructions are just for you, the team's Challenge Advisor; please delete them once you have completed the steps below.**
>
> We've pre-populated this Challenge Project Overview page — which is what will be shared with your Break Through Tech student team in August — using the details from your submission form. You should have received an email inviting you to join this repo as a Collaborator, enabling you to add files and make edits.
> 
> In order for your project to be finalized and assigned to a team, please:
> 1. **Review all sections below** and update or expand any content as needed, making sure to address the SME Feedback in the section immediately below. Look for square brackets to find the places below that require additional inputs from you (e.g., "About [Company / Org Name]").
> 2. **Add your dataset** to the [data folder](data) in this repo.
> 3. **Close the Issue assigned to you in this repo** to let us know that you have made your edits and the overview page is ready for final review. You can do this by going to the _Issues_ tab in the top left section of the menu above, add a comment that says "CA review complete", and click the button to Close the Issue. 
>
> If you're unfamiliar with how to edit a page like this in GitHub, check out [this tutorial](https://ubc-lib-geo.github.io/gis-workshop-waml-template/content/handson/edit-readme.html) for a quick overview (start with step 2 and only edit this page), and [this guide](https://ubc-lib-geo.github.io/gis-workshop-waml-template/content/markdown.html) on how to use Markdown to compose text.
>
>
> ❌ Remember that this is a public repo. Do NOT include: Proprietary data, PII, API keys, credentials, or anything confidential.

---

## 📋 BTT Internal Evaluation Notes
*(This section is for BTT staff and CAs only — remove before sharing with students)*

### Technical Vetting
| Check | Status | Notes |
| :--- | :--- | :--- |
| Python Compatibility | 🟢 | The project utilizes standard scikit-learn and XGBoost libraries which are fully supported in Google Colab environment. |
| Data Readiness | 🟡 | While public, the datasets (IPEDS, BLS, O*NET, Census) involve complex relational merging across multiple schemas, which will be time-consuming for students. |
| Resource Check | 🟢 | Fits within standard CPU-based compute; no GPUs or paid APIs required. |

### Internal Scores
- **Student Fit Score:** 7/10
- **Technical Depth Score:** 8/10
- **Overall Recommendation:** REVISE

### Advisor Feedback Draft
This project offers a strong opportunity to apply ensemble methods to high-impact social data. To succeed, first, simplify the data ingestion phase by providing a pre-merged 'base' file to avoid 10 weeks of cleaning. Second, implement a strict time-based validation holdout set to ensure the model generalizes to future credential cycles. I recommend we proceed with these scoping adjustments to ensure the dashboard remains a feasible deliverable.

---

# Workforce Pell Opportunity Score: Predicting High-Impact Short-Term Education Programs

**Company / Org:** Other  
**Challenge Advisor:** Beth Davis, bethdavisnc@gmail.com  
**Program:** Break Through Tech AI Studio - Fall 2026  

---

## 🏢 About Other
This project focuses on the intersection of higher education and labor market analytics, aiming to optimize the impact of Workforce Pell grants. The team will collaborate to build data-driven tools that assist policymakers and educational institutions in identifying short-term programs that lead to successful workforce integration.

---

## 🎯 The Challenge
### Project Summary
The team will develop an explainable machine learning model to predict the alignment of short-term education programs with regional labor market demands and Workforce Pell criteria. By leveraging integrated datasets from IPEDS, O*NET, and Census sources, the team will utilize gradient-boosted decision trees and SHAP-based explainability to create an actionable "Opportunity Score." This work will culminate in an interactive dashboard designed to guide equitable investment in high-quality workforce training programs.

### Success Criteria
Model accuracy, precision, recall, and F1 score for classification tasks. ROC-AUC. Cross-validation performance. Ability to identify institutional and regional characteristics associated with Workforce Pell readiness. Generation of an interpretable Workforce Pell Opportunity Score. Production of actionable recommendations.

### Project Milestones
Use these milestones to guide your work. Your team will create a GitHub Projects board to track tasks within each milestone.
| Month | Milestone | Key Activities |
|-------|-----------|----------------|
| **September** | Data Exploration & Preprocessing | Develop scripts for joining heterogeneous datasets using CIP codes; conduct exploratory data analysis to identify data quality gaps and potential outliers. |
| **October** | Feature Engineering & Baseline Modeling | Engineer predictive features related to labor demand and institutional capacity; deploy baseline Logistic Regression and Random Forest models for classification. |
| **November** | Model Optimization & Evaluation | Perform hyperparameter tuning on XGBoost models; conduct cross-validation and verify predictive performance against held-out temporal data. |
| **December** | Insights, Deliverables & Presentation | Finalize the interpretability module using SHAP; deploy the interactive dashboard and synthesize findings into an executive-level presentation for stakeholders. |

> **Note for the team:** Please create a GitHub Projects board in this repository to break these milestones into weekly tasks. Go to the **Projects** tab → **New project** → Choose **Board** → Add columns for each month.

---

## 📊 Dataset
**Name and Source:** Publicly available education and labor market data (IPEDS, College Scorecard, BLS, O*NET, Census ACS)  
**Format:** CSV / Structured Relational  
**Size:** under 1gb  
**Location:** Provided via secure shared folder link upon project commencement.

### Key Details
- Structured relational education, workforce, labor market, and demographic datasets linked through common geographic and program identifiers (datasets include IPEDS, College Scorecard, BLS Occupational Employment Statistics, O*NET, U.S. Census ACS, and CIP code crosswalks).
- Teams must strictly monitor for data leakage between geographic entities and ensure that training sets are split according to chronological credential cycles to prevent performance inflation.

---

## 🛠️ Suggested Approach
**ML Problem Type:** Classification  
**Recommended Libraries:**
- Random Forest
- XGBoost
- Gradient Boosting
- Logistic Regression
**Evaluation Metrics:** Classification accuracy, precision, recall, F1-score, and ROC-AUC; model interpretability metrics via SHAP.

---

## 📚 Resources to Get Started
The following resources will help your team understand the problem space and potential technical approaches for this project:
**Background Reading:**
- U.S. Department of Education Workforce Pell Grant eligibility guidelines and reporting standards.
**Technical Tutorials:**
- Scikit-learn documentation on Ensemble Methods and SHAP documentation for model explainability.
**Code Examples:**
- Sample GitHub repositories showcasing pipeline integration of Census and BLS data.

---

## 🤝 How We'll Work Together
**Check-ins:** During our biweekly 60-min AI Studio Lab Section meeting block (2nd and 4th week of every month)  
**Communication:** Email and designated team Slack/Teams channel.  
**Response time:** Within 48 hours on business days.  
**Recommended Tools:**
- **Coding:** Google Colab Free Tier  
- **Collaboration:** GitHub, Notion  
- **Virtual Meetings:** Zoom, Google Meet  

---

## 🚀 Getting Started
1. **Review this overview document** and note any questions for our first meeting.
2. **Begin reviewing the dataset** using the link provided in the Dataset section.
3. **Read the GitHub Projects documentation** [here](https://docs.github.com/en/issues/planning-and-tracking-with-projects/learning-about-projects/about-projects).

I'm excited to work with you!

---

## ❓ Questions?
Please bring any questions to our first meeting during the week of August 24th (Break Through Tech's Bridge to Studio - Session B).
