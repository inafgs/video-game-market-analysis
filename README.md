# video-game-market-analysis
Developed an exploratory and statistical analysis on 16,000+ video game sales records to identify platforms, genres, and markets with the highest commercial potential for 2017.

# Overview
This project performs an end-to-end exploratory and statistical analysis of the global video game industry using historical sales data (up to 2016). The goal is to identify which platforms, genres, and regional markets hold the highest commercial potential for 2017, providing actionable recommendations for a video game retailer.
The analysis covers data cleaning, trend exploration, regional segmentation, correlation studies, and formal hypothesis testing — translating raw data into concrete business strategy.

# Business Problem
A video game retailer needs to plan its inventory and marketing budget for 2017. To do so effectively, it needs answers to questions like:

Which gaming platforms are growing, and which are declining?
Do critic and user reviews actually drive sales?
Do consumer preferences differ significantly across regions (North America, Europe, Japan)?
Are there statistically significant differences in user ratings between platforms and genres?


Dataset

Source: Historical video game sales records
Size: 16,000+ game titles
Features include: Platform, genre, year of release, critic score, user score, and regional sales figures (NA, EU, JP, Other)


# Tools & Technologies
ToolPurposePythonCore programming languagepandasData manipulation and cleaningNumPyNumerical operationsMatplotlibData visualizationSeabornStatistical plottingSciPy (stats)Hypothesis testingJupyter NotebookDevelopment environment

# Methodology
1. Data Cleaning

Standardized column names to lowercase
Converted data types (year_of_release → Int64, user_score → float)
Handled missing values and replaced non-numeric placeholders (TBD → NaN)
Removed duplicate entries
Engineered a total_sales column by aggregating all regional sales

2. Exploratory Data Analysis

Analyzed the number of game releases per year to identify representative time windows
Evaluated total and average sales by platform, filtering for the 2011–2016 period to ensure relevance
Studied the life cycle of gaming platforms (launch, peak, decline)
Focused on the 2013–2016 window for predictive analysis

3. Platform & Genre Analysis

Identified top platforms by total sales in the relevant period: PS4, Xbox One, 3DS
Visualized platform sales evolution over time using line charts
Analyzed sales distribution by genre using bar charts and box plots

4. Correlation Analysis

Investigated the relationship between critic scores and total sales on PS4
Investigated the relationship between user scores and total sales on PS4
Calculated Pearson correlation coefficients for each pair

5. Regional Segmentation

Compared top 5 platforms and genres across three key regions: North America, Europe, and Japan
Identified that Japan behaves as a distinct market (RPG-dominant, Nintendo-heavy, minimal Xbox presence)

6. Hypothesis Testing
Two formal statistical tests were performed using a significance level of α = 0.05:

Test 1: Do Xbox One and PC users give the same average ratings?

Used Levene's test to assess variance equality, then applied an independent samples t-test
Result: No statistically significant difference found


Test 2: Do Action and Sports games receive different average user ratings?

Same methodology as above
Result: Statistically significant difference confirmed




# Key Findings

PS4 and Xbox One are the most commercially promising platforms for 2017, despite showing early signs of market maturation
Critic scores show a moderate positive correlation with sales — professional reviews matter, but are not the sole driver
North America and Europe share similar preferences (Action, Shooter, Sports genres dominate)
Japan is a fundamentally different market: RPGs lead, portables outperform consoles, and Xbox has virtually no presence
Action games receive more consistent user ratings than Sports games, a statistically confirmed difference


# Business Recommendations

Focus advertising budget on PS4 and Xbox One titles in the Action and Shooter genres for Western markets
Maintain differentiated inventory for Japan, prioritizing RPGs and Nintendo platform titles
Leverage critic scores as a marketing argument — they have a measurable impact on sales volume
Prioritize multi-platform releases to maximize revenue reach, with PS4 as the primary target

