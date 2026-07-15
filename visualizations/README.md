# Visualization Roadmap

## Tools & Stack

| Tool | Purpose | Install |
|------|---------|---------|
| Python + Pandas | Data processing | `pip install pandas` |
| Matplotlib/Seaborn | Static charts | `pip install matplotlib seaborn` |
| Plotly | Interactive charts | `pip install plotly` |
| Streamlit | Web dashboard | `pip install streamlit` |
| Jupyter Notebook | Exploration | `pip install jupyter` |

## Planned Visualizations

### Phase 1: Foundational (Matplotlib/Seaborn)
1. Win-Loss Trend Lines (1876-2025, rolling 10-year win%)
2. Championship Bar Chart (WS + pennant titles by team)
3. Pennant Intensity Heatmap (seasons vs teams)

### Phase 2: Advanced (Plotly)
4. Head-to-Head Matchup Matrix Heatmap (15x15)
5. Championship Drought Bar Chart
6. Win% Distribution by Decade (violin/box plots)

### Phase 3: Interactive (Streamlit)
7. NL Team Trend Explorer Dashboard
8. Dynamic H2H Comparison Tool

### Phase 4: ML/Statistical
9. Monte Carlo Championship Simulator
10. Win Contagion Analysis

## Suggested Notebook Structure
```
notebooks/
├── 01_data_loading.ipynb
├── 02_exploratory_analysis.ipynb
├── 03_franchise_win_trends.ipynb
├── 04_championship_analysis.ipynb
├── 05_head_to_head_matrix.ipynb
├── 06_interactive_dashboard.ipynb
└── 07_statistical_modeling.ipynb
```

## Starter Code
```python
import pandas as pd
import matplotlib.pyplot as plt

df = pd.read_csv('../data/nl_all_time_records.csv')
print(df[['Franchise','Wins','Losses','Win_Pct']].sort_values('Wins', ascending=False))

hist = pd.read_csv('../data/nl_historical_performance.csv')
```