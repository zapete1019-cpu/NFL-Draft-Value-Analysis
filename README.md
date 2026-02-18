# NFL-Draft-Value-Analysis
Analyzing 10 years of NFL draft data to identify which offensive positions and rounds provide best value
NFL Offensive Draft Value Analysis (2014-2023)
Overview
Which NFL draft rounds and positions actually produce the most value? This project analyzes 10 years of NFL draft data to answer that question — combining career longevity, playing time, and position-specific production into a composite value score for every offensive pick from 2014 to 2023.
Built as part of a sports analytics portfolio by a data professional transitioning into the sports industry.

The Question
NFL teams invest enormous resources into the draft. But are early picks always worth it? Do certain positions offer better value in later rounds? And how does a specific team — the Denver Broncos — stack up against the rest of the league when it comes to drafting offensive talent?

Key Findings

Round 1 picks produce significantly more value than later rounds, but the drop-off isn't linear — Round 2 offers surprising efficiency relative to cost
Hit rates decline sharply after Round 2 — the percentage of picks who become quality starters falls dramatically from Round 3 onward
Late-round gems exist — a meaningful number of Round 5-7 picks developed into above-average contributors
RB Round 1 value is inflated by selection bias — only elite RB prospects get drafted that high (McCaffrey, Barkley, Henry), skewing the average upward
Broncos draft performance varies significantly by round compared to league average, with notable strengths and weaknesses by position


Value Score Methodology
Each player received a composite Value Score (0-100) combining:
ComponentWeightDescriptionProduction Score60%Position-specific performance metricsLongevity Score40%Career length and consistency
Production Score by Position:

QB: Passing yards + Passing TDs
RB: Rushing yards + Rushing TDs
WR/TE: Receiving yards + Receiving TDs

Career Categories:

⭐ Star (80-100)
🔵 Above Average (60-80)
🟢 Solid Starter (40-60)
🟡 Backup (20-40)
🔴 Bust (1-20)
⚫ Never Played (0)


Note: Analysis is limited to offensive positions (QB, RB, WR, TE). Defensive player analysis requires different data sources (snap counts, advanced defensive metrics) and is identified as a future enhancement.


Visualizations
Value by Draft Round
Average value score broken down by round, showing production vs. longevity components side by side.
Position x Round Heatmap
Which positions are "safe" picks in which rounds? This heatmap shows average value score by position and round combination.
Pick Number vs. Value Scatter
Every draft pick plotted by pick number and career value, with trend line showing the curve of expected value across the draft.
Broncos vs. League Average
Denver Broncos draft efficiency compared to league average by round — their strengths and weaknesses as a drafting organization.
Success Rate by Round
What percentage of picks in each round become quality starters? A stacked bar chart showing outcome distribution (Star → Never Played) by round.
Production vs. Longevity
Do high-production players have shorter careers? This scatter plot examines the relationship between career length and performance output.

Tools & Technologies
ToolPurposePythonCore programming languagePandasData manipulation and analysisnfl_data_pyNFL data source (draft picks, rosters, stats)MatplotlibVisualizationSeabornStatistical visualizationJupyter NotebookDevelopment environmentPower BIDashboard development

Data Sources

nfl_data_py — Draft picks, seasonal rosters, and player performance statistics
Years covered: 2014-2023 NFL Draft classes


How to Run
Prerequisites:
bashpip install nfl_data_py pandas numpy matplotlib seaborn
Steps:

Clone this repository
Open NFL_Draft_Analysis.ipynb in Jupyter Notebook
Run all cells from top to bottom
Data will download automatically via nfl_data_py (~2-3 minutes first run)


Project Structure
NFL-Draft-Value-Analysis/
│
├── NFL_Draft_Analysis.ipynb     # Main analysis notebook
├── draft_analysis_clean.csv     # Cleaned, analysis-ready dataset
├── value_by_round.png           # Visualization 1
├── position_round_heatmap.png   # Visualization 2
├── pick_vs_value_scatter.png    # Visualization 3
├── broncos_vs_league.png        # Visualization 4
├── success_rate_by_round.png    # Visualization 5
├── production_vs_longevity.png  # Visualization 6
└── README.md                    # This file

Future Enhancements

Defensive player analysis using snap count data and advanced defensive metrics
Contract value analysis — draft value relative to rookie contract cost
Advanced metrics — Pro Bowl/All-Pro selections as quality indicators
Scouting model — predict draft value from college stats and combine metrics
Extended dataset — incorporate 2024-2025 draft classes as careers develop


About
Built by Zach Peterschmidt — analytics professional with 6+ years of experience in data strategy, predictive modeling, and performance analytics. Former 4-year collegiate soccer player at Johnson & Wales University (Denver campus). Seeking opportunities in sports analytics with Denver-area organizations.