# 🧭 HR Dynamix Dashboard (Tableau)

This project presents a comprehensive **HR analytics dashboard** built in **Tableau**, powered by a **synthetically generated dataset** using **Python (Faker)** and **ChatGPT**. The dashboard is designed to support **HR managers** with both **high-level strategic insights** and **employee-level analysis** for better decision-making.

---

## 🌐 View the Live Dashboard

👉 **[View the HR Dynamix Dashboard on Tableau Public](https://public.tableau.com/views/HRDashboard_17498217280520/HRSummary?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)**  

---

## 🎯 User Story

**As an HR manager**, I want a comprehensive dashboard to analyze human resources data, offering both a **summary view** for overall insights and a **detailed employee records view** for deep-dive analysis.

---

## 📊 Dashboard Structure

### 1. **Summary View**
The Summary View is divided into three sections:

#### 🔍 Overview
- Total number of hired, active, and terminated employees
- Hiring and termination trends across years
- Department-wise and job title-wise employee breakdown
- HQ vs Branch employee distribution *(New York is the HQ)*
- Employee distribution by city and state

#### 👥 Demographics
- Gender ratio across the organization
- Employee distribution by age group and education level
- Total employees in each age group and education level
- Correlation between education levels and performance ratings

#### 💰 Income Analysis
- Salary comparisons across education levels and gender
- Age-salary correlation within each department
- Highlight discrepancies and salary trends by demographic groups

---

### 2. **Employee Records View**
- A filterable list of all employees
- Displays name, department, position, gender, age, education, and salary
- Interactive filtering based on any field for deeper exploration

---

## 🛠️ Data Generation

The dataset was **synthetically created** using a Python script powered by **Faker** and **ChatGPT prompts**, simulating realistic HR records with **8,950 entries**.

### 🔢 Features Included

- `Employee ID`: Unique identifier  
- `First Name`, `Last Name`: Randomized using Faker  
- `Gender`: 46% Female, 54% Male  
- `State & City`: Randomly selected from custom-defined lists  
- `Hire Date`: Generated with custom probability from 2015–2024  
- `Department`: Chosen based on predefined probabilities  
- `Job Title`: Department-dependent job roles with specific likelihoods  
- `Education Level`: Mapped logically to job titles  
- `Performance Rating`: From "Excellent" to "Needs Improvement"  
- `Overtime`: 30% Yes, 70% No  
- `Salary`: Based on job title and department with defined ranges  
- `Birth Date`: Consistent with realistic age & hire date  
- `Termination Date`: Assigned to 11.2% of employees, respecting time gaps  
- `Adjusted Salary`: Calculated using modifiers for gender, education, and age

### 🧠 GPT-Generated Prompt
> “Generate a Python script to simulate a realistic HR dataset with 8,950 employee records including attributes such as Employee ID, name, gender, location, job title, salary, performance, and termination logic…”

The Python code was modular, with clearly documented functions and customizable parameters for reuse in future iterations.

---
