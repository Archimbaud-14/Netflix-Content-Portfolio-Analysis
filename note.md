# 📝 Note: Netflix Content Portfolio Analysis and Strategy Insights

## Methodology

### 1. Data Loading & Cleaning
- Loaded `netflix_titles.csv`: **8,807 titles**, 12 columns
- Handled missing values by filling `director`, `cast`, and `country` with "Unknown"
- Parsed `date_added` into datetime and extracted `year_added` and `month_added`

### 2. Portfolio Transformation
- Exploded the `listed_in` column (split by comma) to accurately count genre distributions
- Filtered primary countries by taking the first country listed in the `country` column
- Grouped by `year_added` and `type` to analyze content strategy shifts over time

### 3. Visualizations

| # | Chart | File |
|---|-------|------|
| 1 | Stacked Bar | Yearly Growth | `chart1_yearly_growth.png` |
| 2 | Area | Content Strategy Shift | `chart2_strategy_shift.png` |
| 3 | Bar | Top 15 Genres | `chart3_top_genres.png` |
| 4 | Grouped Bar | Country Contribution | `chart4_country_contribution.png` |
| 5 | Bar | TV Show Season Distribution | `chart5_season_distribution.png` |
| 6 | Grouped Bar | Rating Distribution | `chart6_rating_distribution.png` |
| 7 | Bar | Monthly Additions | `chart7_monthly_additions.png` |

---

## Key Findings

| Metric | Value |
|--------|-------|
| Total Titles | 8,807 |
| Movie Share | 69.6% |
| TV Show Share | 30.4% |
| Peak Addition Year | 2019 (1,543 titles) |
| Top 3 Countries | USA (2,818), India (972), UK (419) |
| Top Genre | International Movies (2,752) |
| Most Common Rating | TV-MA (3,207 titles) |

---

## 💡 5 Content Strategy Insights

1. **Strategic Shift towards Series:** While the catalog is historically movie-heavy (69.6%), there is a clear strategic shift: before 2015, Movies were ~85% of additions, but by 2019 TV Shows grew to represent 32% of new content.
2. **The "Limited Series" Trend:** 67% of all TV Shows on the platform consist of only 1 season, reflecting a strong preference for limited series and low-commitment content.
3. **Global Sourcing:** The USA leads content origination, but India has grown rapidly as the second-largest contributor, indicating a heavy investment in the Asian market.
4. **Genre Concentration:** International Movies, Dramas, and Comedies form the backbone of the library, vastly outnumbering niche genres.
5. **Seasonal Drops:** October sees the highest volume of content additions, aligning with the traditional fall TV season and holiday ramp-up.

## Technical Stack
- **Python 3.13**: pandas, matplotlib, seaborn, numpy
- **Dataset**: Netflix Titles (8,807 rows)

*Analysis completed May 2026*
