# The-Sophomore-Jinx-Statistical-Analysis-

## Overview
This project investigates the popular sports phenomenon known as the "Sophomore Jinx", which suggests that athletes who perform exceptionally well in their rookie (first) season often perform worse during their sophomore (second) season.

Using Major League Baseball hitter data, we test whether a statistically significant decline exists between rookie-year and sophomore-year performance.

## Objective
Test the hypothesis that a sophomore jinx exists using MLB data.

## Deliverables include:
- Quantitative analysis (statistics + plots)
- Hypothesis testing (paired t-tests)
- Interpretation and reflections on why the phenomenon occurs

## Dataset
File: Hitter Sheet Example.csv
Data includes Rookie of the Year hitters and their:
- Games Played (G)
- At-Bats (AB)
- Batting Average (BA)
- Slugging Percentage (SLG)

## Methods & Quantitative Analysis
1) Data Cleaning
- Removed players with missing sophomore-year statistics.

2) Variables
We calculated performance change variables:
- BA_Diff = Sophomore BA − Rookie BA
- SLG_Diff = Sophomore SLG − Rookie SLG

3) Hypothesis Testing
We used paired t-tests because rookie and sophomore stats are paired measurements for the same players.

## Hypotheses:
- H₀: No difference between rookie and sophomore performance
- H₁: Sophomore performance is worse than rookie performance

## Results (Paired t-test):
Metric | t-statistic | p-value | Conclusion
Batting Average (BA) | -4.22 | 0.0000568 | Significant decline
Slugging Average (SLG) | -4.95 | 0.0000033 | Significant decline

## Both p-values are far below 0.05 → Reject H₀
Conclusion: There is strong statistical evidence supporting the existence of the Sophomore Jinx.

## Visualizations
This project includes:
- Histogram of Batting Average change (BA_Diff)
- Histogram of Slugging Average change (SLG_Diff)
- Both plots include a red reference line at 0 to visually compare improvement vs decline

## Interpretation & Reflection
Although results support the Sophomore Jinx statistically, the phenomenon is best explained by real-world factors such as:
- Regression to the Mean
- Opponent Adjustment
- Pressure & Expectations

Therefore, the jinx is likely not "luck" or superstition, but instead a predictable performance pattern supported by statistics and behavioral factors.

## Tools & Libraries Used
- Python
- Pandas
- Matplotlib
- SciPy

## How to Run (Google Colab)
1. Open Google Colab
2. Upload the file: Hitter Sheet Example.csv
3. Run the notebook/code to reproduce:
   - cleaned dataset
   - hypothesis testing
   - graphs
   - report output

## Project Structure
Sophomore-Jinx-MLB/
├── Hitter Sheet Example.csv
├── Sophomore_Jinx_Analysis.ipynb
├── README.md
└── (optional) The_Sophomore_Jinx_Case_Study.docx

## Author of the Solution Analsysis 
Doha Ahmed Zaky
M.S. Data Science & Artificial Intelligence — Bryant University

## License
This project is for academic use only.

