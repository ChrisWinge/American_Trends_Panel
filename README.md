# 🌹 Political Data Research: Social Justice Initiative Support Index

[cite_start]This project was developed as a portfolio piece for the **Blue Rose Research Data Analyst** role[cite: 1]. [cite_start]The goal was to take complex survey data, clean it rigorously, and produce a concise strategic memo for political decision-makers[cite: 2]. [cite_start]The analysis is contained entirely within the accompanying Jupyter Notebook: **`The Blue Research Group.ipynb`**[cite: 3].

---

### 🎯 Key Strategic Question: The "Winning" Framework

[cite_start]To maximize support for a Progressive Social Justice Initiative focused on immigration and public resources, this analysis answers the most critical questions for any operational leader[cite: 3]:

* [cite_start]**Who to Talk To:** **Moderates** are the highest ROI persuasion target; while Liberals show high baseline support, Moderates represent the swing group necessary for a majority[cite: 5, 12].
* [cite_start]**What to Say:** Use a **pragmatic, neutral message** to appeal to Moderates, and **avoid social justice framing** with traditional Christian groups, who show the highest resistance[cite: 6, 12].
* [cite_start]**Where to Spend:** Resources should focus on moving Moderates, as they are not currently against the initiative but require a carefully framed message to push them into the supportive range[cite: 12].
* [cite_start]**What to Ignore:** **Income levels** should be disregarded for segmentation; the analysis found that support is flat across all income brackets and is not a driver of support[cite: 4, 12].

---

### 🛠️ Technical Workflow & Quality Control (QC)

[cite_start]This project demonstrates core data analyst skills using Python/Pandas to ensure data integrity and create high-value features[cite: 7]:

1. [cite_start]**Data Isolation:** Created a lean **8-column DataFrame** from the original ~140 variables[cite: 7].
2. [cite_start]**Quality Control:** Identified and removed **system missing codes (99)** across all variables, preventing mathematical errors (like the unexpected max score of 396 that was debugged and fixed)[cite: 8].
3. [cite_start]**Feature Engineering:** Built the **SJ_Support_Index** (a composite score ranging 0-10) by aligning and recoding four raw attitude scales into a single, reliable dependent variable[cite: 9].
4. [cite_start]**Segmentation:** Used Pandas **`df.groupby()`** to segment the Index by Ideology, Income, Education, and Religion to produce the final strategic recommendations[cite: 10].

---

### 🛑 Data Source and Licensing Disclaimer

* [cite_start]**Source Data:** Pew Research Center’s American Trends Panel, Wave 151[cite: 11].
* **Dataset Link:** [Download the original data from Pew Research Center](https://www.pewresearch.org/dataset/american-trends-panel-wave-151/)
* [cite_start]**Licensing Note:** The original raw data files (`.csv` and `.sav`) are **NOT** included in this repository due to the Pew Research Center’s licensing restrictions on public distribution[cite: 11].
* **Setup Instructions:** To run the analysis locally, download the `.csv` file from the link above and ensure it is placed in the project directory as `ATP W151.csv`.
* [cite_start]**Disclaimer:** The opinions expressed herein, including any implications for policy, are those of the author and **not of Pew Research Center**[cite: 12].
