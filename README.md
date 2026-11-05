# 📊 Impact of Social Media on Student Life

### End-to-End Data Analytics Mini Project | Excel & Power BI

![Project](https://img.shields.io/badge/Project-Data%20Analytics-blue)
![Excel](https://img.shields.io/badge/Tool-Excel-green)
![Power BI](https://img.shields.io/badge/Tool-Power%20BI-yellow)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📌 1. Project Overview

This mini project focuses on analysing the impact of social media usage on students' academic performance, mental health, sleep duration and stress levels.

The project follows an end-to-end data analytics workflow, starting with raw dataset cleaning and transformation using Microsoft Excel, followed by data modelling, DAX calculations and interactive dashboard development using Power BI.

The objective is to identify social media usage patterns, understand relationships between social media habits and student well-being, and provide meaningful insights that support informed decision-making by teachers, parents and students.

## 🎯 2. Project Objectives

* Analyse student social media usage patterns across different platforms.
* Identify usage trends based on age, gender and academic level.
* Examine the relationship between daily social media usage and sleep duration.
* Understand the relationship between social media usage, stress and mental health.
* Evaluate academic performance across different social media platforms.
* Identify factors associated with student well-being and academic performance.
* Develop an interactive Power BI dashboard for effective data-driven decision-making.

## 📂 3. Dataset Information

**Dataset Source:** [Student Social Media Dataset – Kaggle](https://www.kaggle.com/datasets/harishyadav0506/impact-of-social-media-on-life)

**Domain:** Education / Psychology / Social Media Analytics

**Dataset Description:**

The dataset contains student-level information about social media usage habits, sleep patterns, stress levels, mental health and academic performance.

### Dataset Attributes

| Attribute                   | Description                                         |
| --------------------------- | --------------------------------------------------- |
| Student_ID                  | Unique student identifier                           |
| Age                         | Student's age                                       |
| Gender                      | Gender category                                     |
| Academic_Level              | High School / Undergraduate / Postgraduate          |
| Primary_Platform            | Main social media platform used                     |
| Daily_Usage_Hours           | Average daily social media usage                    |
| Weekend_Extra_Hours         | Additional weekend usage                            |
| Device_Type                 | Device used to access social media                  |
| Sleep_Duration_Hours        | Average sleep duration                              |
| Sleep_Quality_Score         | Sleep quality rating                                |
| Late_Night_Usage            | Whether the student uses social media late at night |
| Social_Comparison_Frequency | Frequency of social comparison                      |
| Perceived_Stress_Score      | Student's perceived stress score                    |
| Mental_Health_Index         | Student's mental health score                       |
| Academic_Performance_GPA    | Student's GPA                                       |
| Overall_Impact              | Overall impact category                             |
| Stress_Level                | Categorized stress level                            |
| GPA_PERFORMANCE_LEVEL       | Categorized academic performance                    |

## 🛠️ 4. Tools & Technologies

**Microsoft Excel**

* Data cleaning and preprocessing
* Handling missing values
* Removing duplicate records
* Data standardization
* IF and logical functions
* VLOOKUP for data extraction
* Pivot Tables for initial analysis
* Fact and Dimension table preparation

**Microsoft Power BI**

* Data import and transformation
* Data modelling and relationships
* DAX calculated columns and measures
* Interactive visualizations
* Key Influencers
* Decomposition Tree
* KPI cards and dashboard development
* Filters, slicers and drill-down

## 🧹 5. Data Cleaning & Preprocessing – Excel

Performed data cleaning and preprocessing to improve data quality and prepare the dataset for analysis.

### Tasks Performed

**1. Data Cleaning**

* Identified and removed duplicate records.
* Checked missing values in important columns.
* Handled missing values in Perceived_Stress_Score and Academic_Performance_GPA.
* Standardized inconsistent text and category values.
* Corrected formatting inconsistencies.

**2. Data Transformation**

Created additional calculated columns using Excel logical functions.

* Stress Level Classification:

  * Low Stress
  * Medium Stress
  * High Stress

* GPA Performance Classification:

  * Low GPA
  * Medium GPA
  * High GPA

**3. Data Preparation**

* Used filtering and sorting to organize records.
* Applied VLOOKUP to extract and combine relevant information.
* Created separate Fact and Dimension tables.
* Used Pivot Tables to summarize student information and identify initial trends.

**4. Fact and Dimension Tables**

Prepared a basic dimensional structure to organize the dataset.

| Table            | Description                                                                     |
| ---------------- | ------------------------------------------------------------------------------- |
| Fact Table       | Student ID, GPA, Perceived Stress Score, Mental Health Index and Sleep Duration |
| DIM_STUDENT      | Student ID, Age, Gender and Academic Level                                      |
| DIM_GPA          | GPA and GPA Performance Level                                                   |
| DIM_STRESS_LEVEL | Perceived Stress Score and Stress Level                                         |

## 🏗️ 6. Data Modelling – Power BI

Imported the cleaned Excel data into Power BI and established relationships between the Fact and Dimension tables.

### Modelling Activities

* Created relationships between Fact and Dimension tables.
* Defined appropriate cardinality.
* Established lookup tables for student, GPA and stress information.
* Organized the data model for efficient reporting and analysis.

**Data Model Screenshot:**

*Add your Power BI data model screenshot here.*

## 📐 7. DAX – Calculated Measures

Created DAX measures to calculate important student performance and well-being indicators.

### Key Measures

| Measure                     | Purpose                             |
| --------------------------- | ----------------------------------- |
| Total Students              | Total unique students               |
| Average Daily Usage         | Average social media usage hours    |
| Average Sleep Duration      | Average student sleep hours         |
| Average Sleep Quality       | Average sleep quality score         |
| Average Mental Health Index | Average mental health score         |
| Average GPA                 | Average academic performance        |
| Average Stress Score        | Average perceived stress score      |
| High Stress Students        | Number of students with high stress |
| Low GPA Students            | Number of students with low GPA     |

### Sample DAX Measures

**Total Students**

```dax
Total Students =
DISTINCTCOUNT(Fcat[Student_ID])
```

**Average GPA**

```dax
Average GPA =
AVERAGE(Fcat[Academic_Performance_GPA])
```

**Average Stress Score**

```dax
Average Stress Score =
AVERAGE(Fcat[Perceived_Stress_Score])
```

**Average Mental Health Index**

```dax
Average Mental Health =
AVERAGE(Fcat[Mental_Health_Index])
```

**Average Sleep Duration**

```dax
Average Sleep =
AVERAGE(Fcat[Sleep_Duration_Hours])
```

*Note: These examples use the Fact table name from the Excel workbook. Adjust table and column references if the names differ in your Power BI model.*

## 📊 8. Analysis & Power BI Dashboard

Developed an interactive Power BI report with five pages to explore different aspects of student social media usage and well-being.

### Dashboard Pages

**Page 1 – KPI Overview**

Displays important student-level performance indicators.

* Total Students
* Average Daily Usage
* Average Sleep Duration
* Average Mental Health Index
* Average GPA
* Average Stress Score

**Page 2 – Charts & Visual Analysis**

Visualizes student behaviour and performance patterns.

* Student distribution by gender.
* Social media platform usage comparison.
* GPA performance by gender.
* Stress score and GPA comparison.
* Sleep and social media usage patterns.

**Page 3 – Key Influencers**

Uses the Power BI Key Influencers visual to investigate factors associated with:

* Mental Health Index.
* Academic Performance (GPA).
* Sleep Duration.

**Page 4 – Decomposition Tree**

Uses the Decomposition Tree to explore how different factors contribute to variations in student outcomes.

Analysis dimensions include:

* Primary Platform
* Age
* Gender
* Academic Level
* Daily Usage Hours
* Stress Level

**Page 5 – Consolidated Dashboard**

Provides a consolidated view of important student insights through interactive visuals and KPI indicators.

### Dashboard Screenshots

*Add screenshots of your Power BI report pages here.*

1. KPI Overview
2. Charts
3. Key Influencers
4. Decomposition Tree
5. Consolidated Dashboard

## 🔍 9. Business Analysis Questions

The project focuses on answering the following six business questions:

1. **Student Distribution:** How are students distributed across different social media platforms, age groups, genders and academic levels?

2. **Platform Usage:** Which social media platform has the highest and lowest average daily usage hours among students?

3. **Student Performance:** Which platforms and student groups have the highest and lowest GPA, Mental Health Index and sleep duration?

4. **Stress Analysis:** How many students fall under Low, Medium and High stress categories, and how does social media usage relate to their stress levels?

5. **Influential Factors:** Which factors, such as daily usage hours, primary platform, age and stress level, are associated with students' mental health, academic performance and sleep duration?

6. **Student Risk Identification:** How can teachers quickly identify students with excessive social media usage, insufficient sleep, high stress and lower academic performance?

## 💡 10. Insights & Conclusions

The analysis aims to generate insights through four levels of analytics.

**1. Descriptive Analytics**

* Understand student social media usage patterns.
* Compare platform popularity.
* Summarize GPA, sleep duration and stress levels.

**2. Diagnostic Analytics**

* Explore relationships between daily usage and sleep duration.
* Examine the association between social media habits and academic performance.
* Identify factors associated with mental health and stress.

**3. Predictive Analytics**

* Explore potential risk patterns using influential factors.
* Identify student groups that may require additional attention.

**4. Prescriptive Analytics**

* Encourage healthy social media usage habits.
* Promote better sleep routines.
* Support student awareness and wellness initiatives.
* Help teachers identify students who may benefit from additional support.

### Conclusion

This project demonstrates the end-to-end data analytics process, from raw data cleaning and preprocessing in Excel to data modelling, DAX calculations and interactive visualization in Power BI.

By analysing social media usage alongside academic performance, mental health, sleep duration and stress levels, the project aims to provide meaningful insights into student well-being.

The interactive dashboard helps teachers, parents and students explore patterns and make more informed decisions to encourage healthier digital habits and improve student wellness.

## 📁 11. Project Files

| File                                          | Description                                                                    |
| --------------------------------------------- | ------------------------------------------------------------------------------ |
| Social_media_impact_on_life Mini Project.xlsx | Excel workbook containing cleaned data, Pivot Tables and Fact/Dimension tables |
| Socialmedia_impact_on_student_life.pbix       | Interactive Power BI report                                                    |

## 🚀 12. Skills Demonstrated

* Data Cleaning & Preprocessing
* Excel Formulas and Functions
* Data Transformation
* VLOOKUP
* Pivot Tables
* Fact and Dimension Modelling
* Power BI Data Modelling
* DAX Measures
* Data Visualization
* Key Influencers
* Decomposition Tree
* Business Intelligence
* Analytical Thinking
* Data Storytelling

## 👩‍💻 About This Project

This mini project is part of my Data Analytics learning journey and portfolio development.

I am an aspiring Data Analyst, continuously developing my skills in Excel, Power BI, data cleaning, data modelling and business analysis.

**Tools:** Microsoft Excel | Power BI

**Project Category:** Data Analytics / Business Intelligence

**Author:** Your Name

---

⭐ If you find this project useful, feel free to explore the repository and share your feedback.
# MINI-PROJECT-1
