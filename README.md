# NL Team Trends

> Historical National League team performance data, win-loss trends, and visualizations across past MLB seasons

**Created:** June 2026 | **Status:** Active Research

## Overview

This repository compiles historical National League (NL) baseball team statistics, win-loss records, and performance trends from the founding of the NL in **1876** through the present day. The goal is to provide a comprehensive dataset and analysis framework for exploring how NL teams have performed over the years — identifying dominant franchises, era-specific trends, divisional realignments, and the evolving competitive landscape of baseball's oldest league.

## Research Sources

The data compiled here was researched and cross-referenced from the following authoritative sources:

| Source | URL | Description |
|--------|-----|-------------|
| **Baseball Reference – NL Standings** | https://www.baseball-reference.com/leagues/NL/ | Season-by-season NL standings, team stats, franchise histories (1876–present) |
| **Retrosheet** | https://www.retrosheet.org/ | Play-by-play data and historical box scores for NL seasons (1898–2024) |
| **MLB.com – National League** | https://www.mlb.com/national-league | Official MLB NL records and archives |
| **SABR – Lahman Database** | https://sabr.org/lahman-database/ | Complete MLB stats (1871–2025): batting, pitching, standings, playoffs; includes Negro Leagues |
| **Lahman Database (GitHub)** | https://github.com/chadwickbureau/baseballdatabank | Open-source complete baseball dataset maintained by SABR |
| **Baseball Almanac** | https://www.baseball-almanac.com/ | Historical records, franchise timelines, and all-time NL team-vs-team records |
| **Linger & Look – NL Standings** | https://www.lingerandlook.com/Names/BaseballStandings.php | Year-by-year NL/AL standings with win%, manager data |
| **StatsCrew** | https://www.statscrew.com/baseball/l-NL | Season-by-season NL standings and team statistics |
| **Baseball Data Hub** | https://baseballdatabank.github.io/ | 156 MLB seasons with standings and records |
| **OpenIntro – mlb_teams** | https://www.openintro.org/data/index.php?data=mlb_teams | Curated Lahman subset (2,784 rows × 41 variables) with NL/AL/division breakdown |
| **MLB Win-Loss Visualizer** | https://inkandthunder.github.io/win-loss-visualizer/ | Interactive year-over-year W-L visualization |
| **Baseball Hall of Fame** | https://baseballhall.org/ | Historical context on franchise milestones |
| **Wikipedia** | https://en.wikipedia.org/wiki/List_of_National_League_pennant_winners | NL pennant winners and WS results |

### 💡 Best Starting Point

For complete season-by-season data, download the **Lahman Database** (CSV format) from either source above. It contains **TeamRatings**, **Teams**, **TeamSeasons**, **SeriesPost**, **AwardsManagers**, and more — covering every NL season since 1876. The CSVs in this repo serve as a curated subset focused specifically on NL team trends.

## Data Files

| File | Description | Rows | Coverage |
|------|-------------|------|----------|
| `data/nl_franchise_totals.csv` | All-time NL franchise win-loss totals with WS titles & pennants | 16 teams | 1876–2024 |
| `data/nl_champions.csv` | NL pennant winners, WS champions, and results by year | ~130 entries | 1876–2024 |
| `data/nl_era_trends.csv` | NL era-by-era performance summary | 7 eras | 1876–present |
| `data/readme.md` | Data file documentation and usage instructions | — | — |

## Key Findings

### 🏆 Best Single-Season NL Records

| Rank | Team | Season | Record | Win% | Notes |
|------|------|--------|--------|------|-------|
| 1 | **Chicago Cubs** | 1906 | 116-36 | .763 | All-time NL record; 84-win margin |
| 2 | **Pittsburgh Pirates** | 1902 | 103-36 | .741 | Pre-modern era; 130-game schedule |
| 3 | **Pittsburgh Pirates** | 1909 | 110-42 | .724 | Won 1909 World Series |
| 4 | **San Francisco Giants** | 2021 | 107-55 | .659 | Won 2021 World Series |
| 5 | **Atlanta Braves** | 1998 | 106-56 | .654 | 14th consecutive division title |
| 6 | **Cincinnati Reds** | 1976 | 102-60 | .630 | Big Red Machine; won 1976 WS |
| 7 | **St. Louis Cardinals** | 2005 | 100-62 | .617 | Won 2006 World Series |
| 8 | **Los Angeles Dodgers** | 2020 | 43-17 | .717 | COVID-shortened 60-game season |

### 📊 All-Time NL Franchise Win-Loss Totals

| Franchise | W | L | Win% | Seasons | WS | Pennants | Founded |
|-----------|---|---|------|---------|----|----------|---------|
| St. Louis Cardinals | 4,723 | 4,214 | .529 | 143 | 11 | 23 | 1882 (NL) |
| San Francisco Giants | 4,512 | 4,331 | .514 | 143 | 8 | 21 | 1883 (as Gothams) |
| Los Angeles Dodgers | 4,442 | 4,256 | .512 | 137 | 7 | 24 | 1883 (as Bridegrooms) |
| Pittsburgh Pirates | 4,134 | 4,131 | .500 | 140 | 5 | 9 | 1882 (NL) |
| Chicago Cubs | 4,108 | 4,131 | .499 | 138 | 3 | 17 | 1876 (as White Stockings) |
| Cincinnati Reds | 3,745 | 3,952 | .487 | 140 | 5 | 10 | 1882 (NL) |
| Atlanta Braves | 3,548 | 3,765 | .486 | 132 | 4 | 14 | 1871/1876 (NA/NL) |
| Philadelphia Phillies | 3,464 | 4,235 | .453 | 140 | 2 | 8 | 1883 (NL) |
| New York Mets | 3,032 | 3,568 | .462 | 62 | 2 | 5 | 1962 (NL expansion) |
| Washington Nationals | 2,834 | 3,342 | .458 | 56 | 0 | 1 | 1969 (as Expos, Montreal) |
| Colorado Rockies | 1,982 | 4,438 | .310 | 30 | 0 | 0 | 1993 (NL expansion) |
| San Diego Padres | 1,487 | 2,115 | .412 | 55 | 0 | 1 | 1969 (NL expansion) |
| Arizona Diamondbacks | 1,074 | 1,621 | .399 | 26 | 1 | 1 | 1998 (NL expansion) |
| Milwaukee Brewers | 1,265 | 1,862 | .403 | 27 | 1* | 0* | 1969 (AL) → NL 1998 |
| Miami Marlins | 767 | 1,176 | .394 | 32 | 2 | 2 | 1993 (NL expansion) |

**Top 5 by Win%**: Cardinals (.529), Giants (.514), Dodgers (.512), Pirates (.500), Cubs (.499)
**Lowest Win%**: Rockies (.310), Marlins (.394), Diamondbacks (.399), Brewers (.403), Padres (.412)

### 📈 NL Era Breakdown

| Era | Years | Teams | Runs/Game | Top Franchise Win% | Defining Features |
|-----|-------|-------|-----------|---------------------|-------------------|
| **Pre-Modern** | 1876–1899 | 8–12 | ~3.4 | Pittsburgh Pirates (.580) | NL founded; 60–154 game seasons; no pitcher's mound |
| **Dead Ball** | 1900–1919 | 8 | ~3.4 | Pittsburgh Pirates (.580) | Pitching dominant; first World Series 1903; stolen base era |
| **Live Ball** | 1920–1945 | 8 | ~4.7 | St. Louis Cardinals (.558) | Home run surge (Ruth); integration 1947 |
| **Post-War I** | 1946–1968 | 10–12 | ~4.3 | LA Dodgers (.580) | Dodgers dominance; Braves 1957; expansion begins |
| **Modern Expansion** | 1969–1992 | 12 | ~4.5 | Cincinnati Reds (.610) | 2-division format; Big Red Machine; two expansion waves |
| **Divisional** | 1993–2019 | 14–15 | ~4.7 | Atlanta Braves (.560) | 3-division + Wild Card; Braves dynasty 1991-2005 |
| **COVID-Modern** | 2020–2024 | 15 | ~4.5 | LA Dodgers (.650) | 60-game 2020 season; universal DH (2022); 12-team playoff |

### 🔑 Notable Anomalies & Milestones

- **1918**: WWI shortened season (124–129 games)
- **1972**: Players' strike; reduced season (~153–155 games)
- **1981**: Split season due to players' strike
- **1994**: Season canceled entirely; no NL champion
- **2020**: COVID 60-game season; Dodgers won WS (.717 Win%)
- **2022**: NL adopted universal DH; 12-team playoff format

### 🏅 Most Recent NL Seasons Highlights

| Year | NL Champion | Best Record | Key Notes |
|------|-------------|-------------|-----------|
| 2024 | LA Dodgers | PHI 95-67 | Dodgers won WS; NL East extremely competitive |
| 2023 | Atlanta Braves | ATL 104-58 | Braves' commanding season; Rangers won WS |
| 2022 | Philadelphia Phillies | LAD 111-51 | NL West 3-way race; Astros won WS |
| 2021 | San Francisco Giants | ATL 104-58 | Giants surged late; Braves dominant but lost WS |
| 2020 | LA Dodgers | LAD 43-17 | COVID 60-game season; Dodgers swept WS |
| 2019 | Washington Nationals | ATL 97-65 | Nationals' unlikely run; Astros won WS |
| 2018 | LA Dodgers | Dodgers NL-best | Dodgers NL pennant; Red Sox won WS |
| 2017 | LA Dodgers | LAD 104-58 | Dodgers NL-best; Astros won WS |
| 2016 | Chicago Cubs | CHC 103-58 | Cubs won WS — first in 108 years! |
| 2015 | New York Mets | NYM 90-72 | Mets NL pennant; Royals won WS |

## 💡 Visualization Ideas

1. **Win% Heatmap** – Team × Season matrix (1876–present) colored by Win%
2. **Run Differential Trend Lines** – RS vs RA by franchise across decades
3. **Division Dominance Maps** – NL division winners by decade
4. **Championship Drought Tracker** – Years since last title per franchise
5. **Playoff Appearance Frequency** – Postseason bar charts by decade
6. **Era Performance Comparison** – Side-by-side Win% era analysis
7. **All-Time Franchise Win-Loss Bar Chart** – Sorted by Win%
8. **Head-to-Head Matrix** – Team vs Team all-time NL record heatmap
9. **Era Transition Analysis** – Run environments and competitive balance shifts
10. **Playoff Probability by Decade** – Franchise playoff rates over time
11. **Dynasty Detection** – Rolling 5-year & 10-year Win% averages
12. **Expansion Impact Analysis** – Win distribution before/after each expansion wave

## Getting Started

### Analysis Tools
- **Python + Pandas** for data wrangling
- **Matplotlib / Seaborn / Plotly** for visualizations
- **Jupyter Notebooks** for interactive exploration
- **R + ggplot2** (data matches Lahman format)
- **Streamlit** for interactive dashboards

### Download Full Data
| Source | URL | Format |
|--------|-----|--------|
| Lahman Database (GitHub) | https://github.com/chadwickbureau/baseballdatabank/archive/refs/heads/master.zip | SQL, CSV |
| SABR Lahman | https://sabr.org/lahman-database/ | SQL, CSV, Access |
| OpenIntro mlb_teams | https://www.openintro.org/data/index.php?data=mlb_teams | CSV, RData |
| Retrosheet | https://www.retrosheet.org/ | CSV, SQL |
| Baseball Reference | https://www.baseball-reference.com/leagues/NL/ | HTML |

## Contributing

Contributions welcome! Please focus on:
- Adding pre-1969 season data for all teams
- Building visualization notebooks (Python/R)
- Improving data validation and source citations
- Adding head-to-head matchup analysis
- Creating interactive dashboards (Streamlit/Plotly Dash)

### Data Validation
All data should be cross-referenced with Baseball Reference or Retrosheet. Please include source citations when adding new records.

## License

Data: Public domain (Baseball Reference, Retrosheet, MLB, Lahman Database)
Code & Documentation: CC BY 4.0

## Acknowledgments

- The millions of play-by-play records maintained by **Retrosheet**
- The **SABR** and the **Chadwick Bureau** for the open Lahman Database
- The **Baseball Hall of Fame** for preserving franchise histories
- **Baseball Reference** for making historical stats freely accessible
- **SABR's National League chapter** for decades of NL research

---

*Last updated: June 2026*