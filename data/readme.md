# NL Team Trends — Data Documentation

This directory contains curated historical National League team performance data compiled from primary baseball reference sources.

## Files

### nl_franchise_totals.csv
All-time win-loss records for every NL franchise from 1876 through 2024. Columns:
- **franchise**: Official franchise name
- **modern_name**: Current team name
- **founded**: Year franchise entered the NL
- **founded_as**: Original team name
- **seasons**: Number of NL seasons played
- **all_time_wins / all_time_losses**: Cumulative regular-season W-L
- **win_pct**: Win percentage
- **ws_titles**: World Series championships won
- **ws_years**: Years of WS titles
- **pens**: Number of NL pennants
- **pens_years**: Years of pennant wins
- **division**: Current NL division
- **notes**: Additional context (relocations, expansions)

**Important**: W-L totals are approximate aggregates sourced from Baseball Reference and the Lahman Database. Verify against official MLB records.

### nl_champions.csv
NL pennant winners and World Series results by year from 1876 through 1968. Columns:
- **year**: MLB season year
- **nl_pennant_winner**: Team that won the NL pennant
- **nl_ws_result**: Result in World Series
- **best_record_team**: Team with best regular-season record
- **best_record**: That team's W-L record
- **notes**: Key events (strike-shortened seasons, no WS, etc.)

### nl_era_trends.csv
NL era-by-era performance summary. Columns:
- **era**: Historical period name
- **years**: Year range
- **team_count**: Number of teams in NL
- **avg_runs_per_game**: Average runs scored per game
- **top_team**: Franchise with highest Win% during era
- **top_team_win_pct**: That franchise's era Win%
- **dominant_franchise**: Primary dynasty/contender team
- **years_with_championship**: Championship years
- **defining_features**: Historical context

## How to Use This Data

### Python
```python
import pandas as pd

fr = pd.read_csv('data/nl_franchise_totals.csv')
print(fr.sort_values('win_pct', ascending=False).head(10))

ch = pd.read_csv('data/nl_champions.csv')
print(ch[ch['year'] >= 2000])

er = pd.read_csv('data/nl_era_trends.csv')
print(er.sort_values('avg_runs_per_game', ascending=False))
```

### R
```r
fr <- read.csv('data/nl_franchise_totals.csv')
ch <- read.csv('data/nl_champions.csv')
er <- read.csv('data/nl_era_trends.csv')
```

## Contributing Data Corrections

If you spot errors, please check the sources and open an Issue or submit a PR.

## Sources
See the main README.md for the full source list.
