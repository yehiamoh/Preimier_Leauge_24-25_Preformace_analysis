# Premier League Performance Analysis Project

A comprehensive data science project analyzing Premier League player statistics for the 2024-25 season. This project focuses on processing and analyzing player performance metrics, including goals, assists, expected goals (xG), and other key performance indicators to derive meaningful insights about player contributions and team dynamics.

## 1. Data Cleaning

### Tools and Libraries

- Python (pandas, numpy)
- Matplotlib for initial data visualization
- Custom data processing functions

### Data Processing Steps

- Loaded raw Premier League data from `fbref_PL_2024-25.csv`
- Standardized column names for per-90-minutes statistics (e.g., 'Gls/90s', 'Ast/90s')
- Handled missing player information with custom dictionary mapping
- Converted age and birth year to appropriate numeric types
- Cleaned nationality data by extracting standardized country codes
- Created new metrics:
  - XG-Overperformance (Goals - Expected Goals)
  - xAG-Overperformance (Assists - Expected Assists)

### Data Samples

#### Raw Data Sample

```csv
Player,Nation,Pos,Age,Born,90s,Gls,Ast,G+A,G-PK,Gls.1,Ast.1,G+A.1,xG,xAG
Erling Haaland,no NOR,FW,23,2000,4.0,6,1,7,5,1.50,0.25,1.75,4.2,0.8
```

#### Cleaned Data Sample

```csv
Player,Nation,Pos,Age,Born,90s,Gls,Ast,G+A,G-PK,Gls/90s,Ast/90s,G+A/90s,XG-Overperformance,xAG-Overperformance
Erling Haaland,NOR,FW,23,2000,4.0,6,1,7,5,1.50,0.25,1.75,1.8,0.2
```

The cleaning process standardized the data format, added new performance metrics, and made the dataset ready for detailed statistical analysis.

## 2. Exploratory Data Analysis (EDA)

### Analysis Focus

- Player Performance Metrics
- Goal Scoring Analysis
- Expected Goals (xG) vs Actual Goals

### Key Visualizations

#### Expected vs Actual Goals Analysis

- Scatter plot analysis of Expected Goals (xG) vs Actual Goals
- Identification of over and underperforming forwards
- Performance visualization using color gradients to highlight goal differentials
- Detailed player annotations for significant performers

### Key Insights

- Visual representation of forward performance relative to expected goals
- Identification of players exceeding or falling short of expected performance
- Clear distinction between consistent performers and outliers
- Enhanced understanding of goal-scoring efficiency across the league
