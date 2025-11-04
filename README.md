# 🥣 Is Granola Healthy?

## Overview
This project explores the **differences in perception between the general public and nutrition experts** on what foods are considered healthy.  
By visualizing paired data on public and expert opinions, it uncovers how aligned (or misaligned) these groups are when judging the healthiness of foods like **granola, chocolate, and red wine**.  
The project demonstrates how clear, well-designed visualizations can communicate contrasting viewpoints effectively.

---

## Objectives
- Compare **public vs. expert opinions** on the healthiness of various foods.  
- Learn to create and refine **paired-data scatter plots** for comparison.  
- Identify foods with the **largest differences in perception**.  
- Showcase data visualization techniques to enhance clarity and storytelling.

---

## Dataset
Two datasets are used for this analysis:  
- `healthy-food-survey-public.csv` – survey data from the **general public**  
- `healthy-food-survey-experts.csv` – survey data from **nutrition experts**

| Column Name | Description |
|--------------|-------------|
| `food` | Name of the food item |
| `yes` | Number of respondents who think the food is healthy |
| `no` | Number of respondents who think the food is unhealthy |
| `no_opinion` | Number of respondents with no opinion |
| `public` / `experts` | Percentage of respondents who consider the food healthy |

Each dataset includes responses for **40 different food items**, ranging from fruits and vegetables to processed and packaged foods.

---

## Key Steps and Analysis

### 1. Data Loading and Cleaning
- Loaded both CSV files into **pandas** dataframes.  
- Calculated the **percentage of “yes” responses** for each food item.  
- Rounded values and kept only the relevant columns (`food`, `public`, `experts`).  

### 2. Merging and Preparation
- Combined both datasets on the `food` column.  
- Created a clean dataframe comparing **public vs. expert agreement** on each food’s healthiness.

### 3. Visualization
- Constructed a **scatter plot** to compare opinions of the public and experts.  
- Applied **Pro Tips** to improve interpretability:
  - Added axis labels and gridlines.
  - Highlighted notable outliers (e.g., *granola*, *red wine*).  
  - Ensured equal axis scaling for direct comparison.  

### 4. Interpretation
- Foods like **apples and oatmeal** were rated healthy by both groups.  
- **Granola and red wine** showed major disagreement — the public rated them healthier than experts did.  
- **White bread and soda** were consistently rated as unhealthy by both groups.

---

## Key Insights
- The general public tends to **overestimate the healthiness** of certain foods marketed as “natural” or “wholesome.”  
- Experts maintain more **consistent, evidence-based assessments**.  
- Visual comparisons clearly reveal **communication gaps** in nutritional understanding.  

---

## Tools & Libraries
- **Python**  
- **Pandas** – for data manipulation  
- **Matplotlib** – for scatter plot visualization  
- **Seaborn** – for style and readability  
- **Jupyter Notebook** – for interactive analysis  

---

## Author
Developed as a **data visualization and perception analysis project**, demonstrating how statistical graphics can highlight the gap between public beliefs and expert opinions in nutrition science.

