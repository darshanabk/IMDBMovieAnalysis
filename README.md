# IMDB Movie Dataset Analysis | [Live Dashboard](https://public.tableau.com/app/profile/darshana.b8538/viz/IMDBMovieAnalysis_17383721644000/IMDBMovieAnalysis)
<p align="left">
  <img src="https://github.com/darshanabk/IMDBMovieAnalysis/blob/main/IMDB.jfif" width="800" title="hover text">
</p>
## Project Overview

This project explores trends and insights from the IMDB movie dataset, analyzing factors like genres, duration, languages, directors, and budgets to understand their impact on IMDB ratings. Using **Microsoft Excel** and **Tableau**, we create interactive visualizations to identify key patterns and trends in the film industry.

## Data Analysis Using Excel & Tableau

### **Excel Analysis**
- **Data Cleaning:**
  - Removed duplicate records and missing values.
  - Verified and corrected inconsistencies in columns such as `Language`, `Country`, `Aspect Ratio`, and `Content Rating`.
  - Handled outliers using **Z-score analysis** for `budget`, `gross`, `duration`, and `imdb_score`.

- **Statistical Calculations:**
  - Used **COUNTIF**, **AVERAGE**, **MEDIAN**, and **STDEV** functions to analyze IMDB scores, budget distributions, and genre trends.
  - Created pivot tables for **Genre-wise and Country-wise movie distribution**.
  - Visualized trends using **histograms and box plots**.

### **Tableau Analysis & Visualizations**

### 1. Average IMDB Score (KPI Chart)
- **Chart Type:** Text KPI Chart
- **Columns:** None
- **Rows:** None
- **Measure Values:** `AVG(imdb_score)`
- **Insight:** Displays the overall average IMDB score, helping to understand general rating trends.

### 2. Budget vs. Gross Scatter Plot
- **Chart Type:** Scatter Plot
- **Columns:** `budget`
- **Rows:** `gross`
- **Size:** `imdb_score` (Bubble size based on rating)
- **Color:** Different color for High vs. Low Budget movies
- **Insight:** Shows the correlation between budget and earnings, highlighting outliers (low-budget movies with high revenue).

### 3. IMDB Score vs. Content Rating
- **Chart Type:** Box Plot
- **Columns:** `content_rating`
- **Rows:** `imdb_score`
- **Insight:** Compares IMDB ratings across different content ratings (PG, R, etc.) to identify which categories receive better scores.

### 4. Total Gross Earnings (KPI Chart)
- **Chart Type:** Text KPI Chart
- **Columns:** None
- **Rows:** None
- **Measure Values:** `SUM(gross)`
- **Insight:** Displays the total revenue generated across all movies, analyzing industry-wide financial performance.

### 5. Average Budget (KPI Chart)
- **Chart Type:** Text KPI Chart
- **Columns:** None
- **Rows:** None
- **Measure Values:** `AVG(budget)`
- **Insight:** Shows the average budget of movies in the dataset, highlighting general spending patterns in the industry.

### 6. Gross Revenue by Year
- **Chart Type:** Bar Chart
- **Columns:** `title_year`
- **Rows:** `SUM(gross)`
- **Color:** Highlight top-grossing years
- **Insight:** Shows how movie revenue trends over the years, identifying profitable years in the film industry.

### 7. IMDB Score Trend Over Time
- **Chart Type:** Line Chart
- **Columns:** `title_year`
- **Rows:** `AVG(imdb_score)`
- **Color:** Trendline to show rating movement over time
- **Insight:** Identifies if IMDB scores have improved or declined over the years, revealing trends in viewer preferences.

### 8. Movie Count by Country (Map Chart)
- **Chart Type:** Filled Map (Choropleth)
- **Columns:** `country`
- **Rows:** `COUNT(movie_title_crt)`
- **Color:** Darker shades for countries producing more movies
- **Insight:** Highlights top movie-producing countries and helps analyze geographical dominance in filmmaking.

## Tech Stack
- **Microsoft Excel 2022:** Data analysis, visualization, and statistical calculations.
- **Tableau:** Interactive data visualization.

## Key Insights

- **Genre Impact:** Biography movies tend to have higher IMDB scores, while Horror movies score lower on average.
- **Budget vs. Earnings:** High-budget movies often earn more, but exceptions exist where low-budget films outperform expectations.
- **Content Ratings Influence:** Certain content ratings correlate with higher or lower average IMDB scores.
- **Geographical Trends:** The USA dominates movie production, but some countries specialize in niche genres.

## Conclusion

This project provides valuable insights into how different factors affect IMDB ratings, helping film producers and marketers make more informed decisions.

## Resources
- **Raw Dataset:** [IMDB Movie Dataset](https://github.com/darshanabk/IMDBMovieAnalysis/blob/main/RawData/IMDB_Movies.csv)
- **Excel Workbook:** [IMDB Movie Excel Analysis](https://github.com/darshanabk/IMDBMovieAnalysis/blob/main/DataCleaningAndAnalysis/DataCleaning%20and%20Analysis%20-%20IMDB_Movies.xlsx)
- **Cleaned Dataset:** [IMDB Movie Cleaned Dataset](https://github.com/darshanabk/IMDBMovieAnalysis/blob/main/DataCleaningAndAnalysis/IMDBCleanedDataset.xlsx)
- **Tableau Dashboard:** [Live Dashboard](https://public.tableau.com/app/profile/darshana.b8538/viz/IMDBMovieAnalysis_17383721644000/IMDBMovieAnalysis)






