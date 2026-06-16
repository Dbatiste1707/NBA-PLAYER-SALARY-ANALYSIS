# NBA-PLAYER-SALARY-ANALYSIS
evaluation of how salary correlates to player performance and which players of over and under performing according to what salary they are getting
NBA Salary vs Performance Analysis
Project Overview

This project analyzes NBA player salaries and on-court performance during the 2024–25 season to identify which players provide the best value relative to their contracts. Using Python, Pandas, Matplotlib, and the NBA API, I combined salary and performance datasets, created custom evaluation metrics, and visualized player value across the league.

Objectives
Compare NBA player salaries to on-court production.
Identify the highest-value and lowest-value contracts.
Create custom performance and value metrics.
Visualize the relationship between salary and production.
Tools and Libraries
Python
Pandas
Matplotlib
NumPy
NBA API
Skills Demonstrated
Data Collection
Data Cleaning
Data Merging
Feature Engineering
Data Visualization
Exploratory Data Analysis (EDA)
Sports Analytics
Business Analytics
Data Collection

Player statistics were collected using the NBA API and included:

Points Per Game (PTS)
Rebounds Per Game (REB)
Assists Per Game (AST)

Salary information was combined with player performance data using Pandas merge operations.

The final dataset included 25 NBA players.

Analysis Performed
1. Data Cleaning
Selected relevant player statistics.
Standardized player names across datasets.
Removed unnecessary columns.
2. Data Merging

Combined salary and performance datasets using:

pd.merge()

This allowed player salaries and statistics to be analyzed together.

3. Feature Engineering

Created a custom Performance Score:

Performance Score = PTS + REB + AST

Created a custom Value Score:

Value Score = Performance Score / Salary (Millions)

The Value Score measures how much production a player provides for every million dollars of salary.

4. Data Visualization

Created visualizations including:

Salary vs Performance scatter plot
Top 10 NBA Value Contracts bar chart
Key Findings
Highest Value Contracts
Paolo Banchero
Victor Wembanyama
Shai Gilgeous-Alexander
Jayson Tatum
Luka Dončić
Lowest Value Contracts
Bradley Beal
Jimmy Butler III
Stephen Curry
Jaylen Brown
Kevin Durant
Interpretation

The analysis suggests that younger stars on rookie-scale contracts provide significantly more production relative to salary than many veteran superstars.

Players such as Paolo Banchero and Victor Wembanyama ranked highest because they produce at an All-Star level while earning substantially less than max-contract veterans.

The model also highlights the limitations of purely statistical analysis. Factors such as defense, leadership, playoff performance, and marketability are not included in the Value Score and may affect a player's overall value to a team.

Conclusion

This project demonstrates how data analytics can be applied to sports business decisions. By combining salary and performance data, I developed custom metrics that identify which players provide the greatest production relative to cost. The project highlights the importance of feature engineering, data visualization, and business-focused analytics when evaluating player contracts.

Future Improvements
Include advanced statistics such as PER and True Shooting Percentage.
Analyze all NBA players instead of a sample.
Pull salary data automatically from an online source.
Compare value across multiple NBA seasons.
Build predictive models for future contract value.
Repository Structure

NBA-SALARY-ANALYSIS/

├── README.md

├── nba_salary_analysis.ipynb

├── salary_vs_performance.png

└── top10_value_contracts.png

How to Run
Clone the repository.
Install required libraries:

pip install pandas matplotlib numpy nba_api

Open nba_salary_analysis.ipynb
Run all cells.
