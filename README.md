# 🌹 Political Data Research: Social Justice Initiative Support Index

This project was developed as a portfolio piece for a Data Analyst role. The goal was to take complex survey data, clean it rigorously, and produce a concise strategic memo for political decision-makers. The analysis is contained entirely within the accompanying Jupyter Notebook: **`Social Justice.ipynb`**.

---

### 🎯 Key Strategic Question: The "Winning" Framework

To maximize support for a Progressive Social Justice Initiative focused on immigration and public resources, this analysis answers the most critical questions for any operational leader:

* **Who to Talk To:** **Moderates** are the highest ROI persuasion target; while Liberals show high baseline support, Moderates represent the swing group necessary for a majority.
* **What to Say:** Use a **pragmatic, neutral message** to appeal to Moderates, and **avoid social justice framing** with traditional Christian groups, who show the highest resistance.
* **Where to Spend:** Resources should focus on moving Moderates, as they are not currently against the initiative but require a carefully framed message to push them into the supportive range.
* **What to Ignore:** **Income levels** should be disregarded for segmentation; the analysis found that support is flat across all income brackets and is not a driver of support.

---

### 🛠️ Technical Workflow & Quality Control (QC)

This project demonstrates core data analyst skills using Python/Pandas to ensure data integrity and create high-value features:

1. **Data Isolation:** Created a lean **8-column DataFrame** from the original ~140 variables.
2. **Quality Control:** Identified and removed **system missing codes (99)** across all variables, preventing mathematical errors (like the unexpected max score of 396 that was debugged and fixed).
3. **Feature Engineering:** Built the **SJ_Support_Index** (a composite score ranging 0-10) by aligning and recoding four raw attitude scales into a single, reliable dependent variable.
4. **Segmentation:** Used Pandas **`df.groupby()`** to segment the Index by Ideology, Income, Education, and Religion to produce the final strategic recommendations.

---

### 🛑 Data Source and Licensing Disclaimer

* **Source Data:** Pew Research Center’s American Trends Panel, Wave 151.
* **Dataset Link:** [Download the original data from Pew Research Center](https://www.pewresearch.org/dataset/american-trends-panel-wave-151/)
* **Licensing Note:** The original raw data files (`.csv` and `.sav`) are **NOT** included in this repository due to the Pew Research Center’s licensing restrictions on public distribution.
* **Setup Instructions:** To run the analysis locally, download the `.csv` file from the link above and ensure it is placed in the project directory as `ATP W151.csv`.
* **Disclaimer:** The opinions expressed herein, including any implications for policy, are those of the author and **not of Pew Research Center**.
