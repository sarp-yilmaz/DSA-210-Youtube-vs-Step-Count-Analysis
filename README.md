# Analysis of the Relationship Between YouTube Usage and Daily Step Counts

This repository contains an in-depth analysis of the relationship between daily YouTube usage and daily step counts, supported by data visualization, hypothesis testing, and statistical analysis.

---

## Overview
The goal of this project is to determine whether there is a significant relationship between daily YouTube usage (number of videos watched) and physical activity (measured by step counts). The analysis uses statistical methods, correlation analysis, and hypothesis testing to arrive at a conclusion.

---

## Dataset

### 1. YouTube Watch History
- **Source**: Exported YouTube watch history file.
- **Processed Variables**:
  - `Timestamp`: Date and time of video watched.
  - `Day`: Day of the week.
  - `Hour`: Hour of the day.
  - Aggregated metrics: Daily and hourly counts of videos watched.

### 2. Step Count Data
- **Source**: Health app XML export.
- **Processed Variables**:
  - `date`: Date of recorded steps.
  - `steps`: Total steps recorded per day.
  - `Day`: Day of the week.
  - Aggregated metrics: Daily step counts.

---

## Methods

### 1. Data Cleaning and Preprocessing
- Converted timestamps to consistent date-time formats.
- Aggregated data by day and hour for both datasets.
- Removed outliers based on statistical thresholds.

### 2. Visualizations
The project includes the following visualizations:
- **Daily Trends**:
  - Line plots for daily YouTube views and step counts.
- **Hourly Trends**:
  - Bar plots for hourly YouTube views.
  - Side-by-side line plots comparing hourly YouTube views and steps.
- **Correlation Heatmaps**:
  - Correlation between daily YouTube views and step counts.
  - Correlation between hourly data.
- **Scatter Plots**:
  - Scatter plot with a fitted regression line for daily YouTube views vs. step counts.

### 3. Statistical Analysis
- **Correlation Analysis**:
  - Used Pearson correlation coefficient to measure the linear relationship between variables.
- **Hypothesis Testing**:
  - Null Hypothesis (ℎ₀): There is no significant relationship between daily YouTube usage and step counts.
  - Alternative Hypothesis (ℎ₁): There is a significant relationship between daily YouTube usage and step counts.
  - Significance Level (α): 0.05.
  - Test Results:
    - p-value: Computed from the correlation test.
    - Conclusion: Fail to reject the null hypothesis as p > α.

---

## Results

### Key Findings:
1. **Correlation Coefficient**:
   - Daily YouTube views and step counts showed a weak negative correlation (-0.22).
   - Hourly YouTube views and step counts showed negligible correlation (0.05).
2. **Hypothesis Test**:
   - p-value: 0.1653 for daily data, indicating no significant relationship.
   - The null hypothesis (ℎ₀) was not rejected.
3. **Outliers**:
   - Days with extreme YouTube views or step counts were identified and visualized separately.

---

## Folder Structure

```
root
├── data
│   └── youtube_watch_history.html
│   └── step_count_data.xml
├── notebooks
│   └── analysis.ipynb
├── visualizations
│   └── plots
├── presentation
│   └── hypothesis_analysis.pptx
└── README.md
```

---

## Instructions

### Prerequisites
- Python 3.8+
- Required libraries:
  - pandas
  - matplotlib
  - seaborn
  - scipy
  - numpy
  - python-pptx (for presentation generation)

### How to Run
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Execute the Jupyter notebook:
   ```bash
   jupyter notebook notebooks/analysis.ipynb
   ```
4. View visualizations in the `visualizations/plots` folder.
5. Open the presentation in `presentation/hypothesis_analysis.pptx`.

---

## Conclusion
While the analysis shows some patterns in YouTube usage and step counts, no significant statistical relationship was found between the two variables. This indicates that the two behaviors are likely independent under the observed conditions.

---

## Future Work
- Explore non-linear relationships.
- Incorporate additional data, such as device usage patterns or other physical activity metrics.
- Conduct analysis across different time periods for broader generalization.

---

## License
This project is licensed under the MIT License. See the LICENSE file for details.

---

## Acknowledgments
- Data provided by YouTube and Health app exports.
- Libraries used: `pandas`, `matplotlib`, `seaborn`, `scipy`, `numpy`, and `python-pptx`.

