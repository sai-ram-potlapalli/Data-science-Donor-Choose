# DonorsChoose Project Approval Prediction

## Problem Statement

DonorsChoose.org, a nonprofit platform that helps public school teachers fund classroom projects, is expecting nearly **500,000 project proposals** next year. This surge presents challenges in:

- **Scalability**: Manual screening processes cannot keep up with the volume.
- **Consistency**: Ensuring fair and uniform evaluation across volunteers.
- **Resource Allocation**: Focusing limited volunteer time on proposals that need the most attention.

To address these, this project aims to build a **predictive model** that can estimate the likelihood of a project proposal being approved based on historical data, project metadata, and teacher-submitted essays.

---

## 🧠 Objective

Develop a machine learning model to:
- Predict the **approval status** (`Approved` or `Rejected`) of each project proposal.
- Help DonorsChoose.org **streamline and scale** their vetting process.
- Enhance **consistency** and optimize **volunteer resource allocation**.

---

## 🔍 Why Automate the Vetting Process?

### ✅ Need
- Manual review is **time-consuming** and **not scalable**.
- Variability in reviews can lead to **inconsistent outcomes**.
- Volunteers’ time must be used **strategically and effectively**.

### 🚀 Use
| Category          | Automation Benefit |
|------------------|---------------------|
| **Scalability**   | Automatically screen proposals to handle large volumes. |
| **Consistency**   | Apply standardized, data-driven vetting rules. |
| **Resource Allocation** | Identify borderline proposals and focus volunteer review there. |

---

## 🎯 Benefits of the Predictive Model

- **Operational Efficiency**: Faster screening and quicker posting of approved proposals.
- **Improved Teacher Experience**: Transparent, consistent, and timely feedback.
- **Volunteer Optimization**: Direct effort toward proposals that need the most scrutiny.
- **Data-Driven Insights**: Uncover patterns in successful proposals to guide future submissions.

---

## 📂 Dataset Overview

### `train_data.csv`
Contains metadata and textual information about each project.
- `project_essay_1` to `project_essay_4`: Teacher-submitted narratives
- `project_subject_categories`, `grade_category`, `school_state`, etc.
- `project_is_approved`: Target label (1 = approved, 0 = rejected)

### `resources.csv`
Contains the details of resources requested per project.
- `description`, `price`, `quantity`
- Will be used to compute **project cost** as a key feature

---

## 🛠️ Key Steps in the Project

1. **Data Cleaning** & Feature Engineering
2. **Exploratory Data Analysis** (EDA)
3. **Text Preprocessing** for essays
4. **Model Training** (e.g., Logistic Regression, XGBoost)
5. **Evaluation** using metrics like Accuracy, ROC-AUC
6. **Insights** and recommendations for implementation

---

## 📊 Sample Insights (from EDA)

- Projects with **lower costs** and **experienced teachers** are more likely to be approved.
- Essay **length and clarity** show moderate correlation with approval.
- Subject categories like "Math & Science" have **higher success rates**.

---

## 🤖 Tools & Technologies

- Python (Pandas, Scikit-learn, XGBoost, NLTK)
- Matplotlib, Seaborn (for EDA and visualization)
- Jupyter Notebook
- Git & GitHub

---

## 📈 Business Impact

Implementing this model can help DonorsChoose.org:
- Process 500K+ proposals annually **without additional human load**
- Offer **fairer and faster** experiences for teachers
- Use volunteers **where they’re needed most**

---

## 🙌 Acknowledgments

Thanks to [DonorsChoose.org](https://www.donorschoose.org) for the open dataset and opportunity to solve a meaningful real-world problem.

---
