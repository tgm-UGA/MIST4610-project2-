# MIST4610-project2-
# Team Name :
63756 Group 2

# Team Members 
  1. Afaf Khurram [@Ak87319](https://github.com/ak87319) 811285986

  2. Amber Um [@Asu34123](https://github.com/asu34123) 811142263

  3. Tyler Meyer [@tgm-UGA](https://github.com/tgm-UGA) 811444595

# About Our Dataset 
This dataset includes every real estate transaction with a sale price of $2,000 or more that occurs each year between October 1st and September 30th. Each sale record provides details such as the town, property address, sale date, property type (residential, apartment, commercial, industrial, or vacant land), the sale price, and the property’s assessed value. For residential properties, the dataset also includes information about the specific type of home, such as whether it is a single-family, two-family, or three-family residence, or a condominium. This additional detail allows for more precise comparisons across different categories of residential housing and helps identify trends in demand and pricing for each property type. The data is obtained from the Office of Policy and Management and is collected in accordance with Connecticut General Statutes.

# Question Description
Our team developed two primary research questions for this project. 
The first question is: “How do towns’ median assessed and sale values compare to the statewide median across different years, and which towns consistently rank above or below the statewide trend? In other words, in which towns do properties have greater relative value? Which towns have property values that grow the most over time?” This question is important because differences between assessed values and sale prices can reveal meaningful economic patterns such as regional housing demand, wealth distribution, and local economic growth. Understanding which towns consistently exceed or fall below statewide property value trends provides insight into affordability, tax base strength, and long-term community development. This ties directly to our dataset because it includes annual assessed values, sale prices, and town identifiers, allowing us to calculate medians, compare them across years, and determine which towns show the strongest or weakest value growth relative to the state.

The second question is: “Which property type sells closest to its assessed value? Which properties are over assessed? Which properties are underassessed? Are there any overall trends for towns that are consistently over/under assessed in property value? Which towns have more of a specific property type? For residential properties, what type of residential types are being sold? How do property valuation accuracy and sales patterns vary across towns and property types?” This question is important because valuation accuracy affects tax fairness, municipal revenue, and homeowner equity. Identifying which property types are consistently over- or under-assessed can highlight systemic issues in the assessment process or differences in how certain market segments behave. Understanding which towns sell more of specific property types also adds a demographic and cultural dimension to the analysis, showing how community composition affects property markets. This question connects strongly to our dataset because it includes assessed values, sale prices, detailed property classifications, and town-level information, enabling us to compare assessment accuracy and sales trends across property types and locations.

# Manipulations Applied to the Dataset
We cleaned the dataset to remove irrelevant information and added several new columns to make analysis easier and more meaningful. First, we created a sold_yr column that extracts the year of the sale, improving readability. We also added a year_diff column to measure how long a property was on the market before it sold, which helps indicate which properties may have been more or less desirable to buyers.

Additionally, we created a sr_dec column representing the sales ratio in decimal form. This ratio compares the sale price to the assessed value. Values below 1 indicate the property sold for less than its assessed value, while values above 1 indicate it sold for more. This metric makes it easy to evaluate how properties performed relative to their assessments and to identify patterns in the market.

We also identified three properties with sale dates in the 1900s, which were significant outliers and skewed our analysis. To ensure more accurate visualizations, we removed these records from the dataset.

Together, these allow for clearer insights into property desirability, valuation accuracy, and overall market dynamics.

# 📊 DASHBOARD 1 — 
Town Value Trends Over Time 
### Dashboard 1 Screenshot
<img width="311" height="339" alt="Screenshot 2025-11-17 at 11 40 49 PM" src="https://github.com/user-attachments/assets/bc4bc5cf-71d3-4aa2-ba01-9aacdcb6bd1c" />

This visualization provides the statewide median sale price for all Connecticut real estate transactions and serves as the foundational benchmark for evaluating local markets. By establishing this statewide reference value, we can meaningfully compare how individual towns perform relative to the average property sale price across the entire state. A town’s position above or below this value helps identify whether the local market is considered high-value, average, or lower-value. High-value areas typically reflect strong buyer demand, higher-income populations, and competitive housing markets, while towns below the median may offer more affordability or reflect slower economic growth. Understanding this statewide benchmark is crucial for all visualizations that follow, as it allows us to contextualize which towns outperform or underperform the statewide housing market.

## Visual 2 — Statewide Median Assessed Value (Scorecard)
<img width="317" height="340" alt="Screenshot 2025-11-17 at 11 41 25 PM" src="https://github.com/user-attachments/assets/c9412ccd-1040-434b-bc1e-b5f28c8ae032" />

This visualization displays the statewide median assessed value assigned by municipalities for tax purposes. Comparing statewide assessed values to statewide sale prices is essential for determining whether Connecticut property assessments are generally aligned with the market. If assessed values fall well below sale values statewide, this suggests widespread undervaluation, which can have implications for municipal revenue and taxation fairness. Conversely, a close alignment signals strong valuation accuracy. This visualization forms the baseline for understanding valuation differences across towns later in the dashboard. It is also the foundation for studying property tax fairness and identifying regions where assessments lag behind market conditions, potentially requiring reassessment.

## Visual 3 — Median Sale Value by Town (Bar Chart)
(insert dashboard 3 image here)

This visualization ranks each town by its median sale price, revealing which areas have the highest and lowest property markets. Towns such as Greenwich, Darien, and New Canaan clearly emerge as the strongest markets, with substantially higher median sale prices than most other towns. These high-value towns exhibit strong demand, often linked to affluent populations, competitive school districts, higher incomes, and limited housing supply. On the opposite end, towns with lower sale medians reflect more affordable living, possibly due to lower demand, more available housing stock, or weaker local economic conditions. This visualization helps identify geographic housing disparities, highlighting how wealth and property value concentrate in certain communities while others remain more affordable. It also sets the stage for analyzing how these value levels relate to assessed values and year-to-year trends in subsequent visualizations.

## Visual 4 — Difference Between Median Sale and Median Assessed Value by Town
(insert image 4 here)

This visualization highlights the gap between each town’s median sale price and its median assessed value. Towns with very large positive gaps—such as Darien, New Canaan, and Greenwich—show that properties consistently sell for much more than towns assess them for. This indicates strong demand combined with potentially outdated assessments. The result is an undervaluation pattern that affects tax fairness and municipal revenue. Towns with smaller gaps or near-zero differences demonstrate more accurate assessments aligned with market behavior. This visualization is critical because it uncovers where valuation inaccuracies are most significant and which markets are hottest relative to their assessed worth. Buyers may find better deals in towns with smaller gaps, while municipalities with large gaps may need to update assessments to maintain tax fairness and revenue stability. Investors can also use this information to identify markets where real property value far exceeds tax valuation.

## Visual 5 — Statewide Median Sale Value Over Time (Line Chart)
(insert image here)

This line chart tracks the statewide median sale price across all years in the dataset, revealing Connecticut’s broader housing market trajectory. A consistently rising line indicates strong appreciation, meaning homes across the state are increasing in value over time. Periods of stagnation or decline may correspond to economic events, policy changes, or shifts in buyer preferences. This visualization is important because it establishes the statewide trend that individual towns can be compared against. Towns growing faster than the statewide trend are increasing in desirability or market pressure, while towns growing slower may be facing stagnation. Understanding the statewide context allows us to interpret whether local town trends represent strong outperformance, normal movement, or weaker demand.

## Visual 6 — Heatgrid of Median Sale Value by Town and Year
This heatgrid visualizes median sale values for each town across each year, with darker colors representing higher sale values. It is one of the most powerful visuals because it shows both cross-town variation and year-to-year market changes simultaneously. Towns with consistently dark shading represent stable high-value markets. Towns that darken over time represent emerging markets experiencing rapid appreciation. Meanwhile, towns with lighter or inconsistent colors reflect more affordable markets or fluctuating demand. This visualization clearly identifies patterns such as which towns are booming, which are stable, and which may be declining. It allows investors, policymakers, and analysts to spot long-term housing trends, identify emerging hot markets, and detect regions where property values have remained stagnant.

# 📊 DASHBOARD 2 — Property Type & Assessment Accuracy (5 Visuals)
### Dashboard 2 Screenshot

## Visual 1 — Residential Type Sales Count
![D2 Visual 1](https://raw.githubusercontent.com/ak87319/MIST4610-project2-/e0a8af246020625d88fa150e2942ec86e069da9c/D2%20Vis%201.png)
This visualization displays how many properties were sold for each residential subtype (such as single-family homes, condos, and multi-family homes). It clearly shows that single-family homes dominate the Connecticut housing market, followed by condominiums and smaller multi-family units. This pattern reflects buyer preference, zoning composition, and the overall distribution of housing stock across the state. The large volume of single-family home sales indicates that most residential real estate activity revolves around traditional suburban-style housing. For policymakers, this suggests that changes in zoning, development planning, or tax assessment policies should prioritize single-family housing. For investors, this provides insight into the property types with the highest turnover and the greatest market demand. Understanding the distribution of sales also helps contextualize later visualizations on assessment accuracy and property value relationships.

## Visual 2 — Median Sales Ratio by Property Type
(insert visual 2 here)

This visualization compares median sales ratios across all major property types. The sales ratio is calculated as sale price divided by assessed value, meaning values below 1 indicate that properties typically sell for more than their assessment, while values near 1 indicate accurate assessments. This chart reveals which property types are systematically undervalued or overvalued by municipal assessment systems. For example, certain property types like commercial or public utility properties may show very low ratios, signaling chronic undervaluation. Residential properties may show more stability but still indicate slight undervaluation. This visualization matters because valuation accuracy directly impacts tax fairness, municipal budgeting, and real estate investment behavior. If some property categories show large deviations from their assessed values, it could signal the need for reassessment or policy reform. Investors may use this insight to identify undervalued property types with potential for strong returns.

## Visual 3 — Sales Ratio by Town and Year (Heatgrid)
(insert visual 3 here)
This heatgrid displays assessment accuracy for each town across each year, using the median sales ratio as the measurement. Darker colors indicate ratios closer to or above 1 (accurate or slightly over-assessed), while lighter colors indicate undervaluation. This visualization helps identify towns that consistently under-assess homes relative to their market value, as well as towns whose assessment accuracy fluctuates between years. These patterns can reveal systematic issues in local tax assessment practices, shifting market conditions, or unique local characteristics affecting sale prices. For example, towns with persistently lighter shades may have outdated assessments failing to reflect growing market demand. Meanwhile, towns with darker consistent shades are valuing homes more accurately. This helps municipalities improve tax fairness and informs property owners about potential discrepancies in their assessments.

## Visual 4 — Assessed Value vs Sale Price (Scatter Plot)
(insert visual 4 here)

This scatter plot compares each town’s median assessed value to its median sale value, with each point representing a town. Ideally, points should fall along a 45-degree line where assessed values equal sale prices. Towns above the line have properties that routinely sell for more than their assessed value, indicating undervaluation. Towns on the line have accurate assessments, while towns below the line (if any) would indicate overvaluation. This visualization is important because it allows us to directly assess how fair and accurate municipal property valuations are across towns. It also illustrates how market behavior diverges from tax records, highlighting regions where housing demand outpaces government assessments. For investors, this chart shows where market value significantly exceeds assessed value, signaling high-demand areas. For policymakers, it highlights where reassessment could improve tax fairness.

## Visual 5 — Sales Ratio Over Time by Property Type (Line Chart)
(insert visual 5 here)

This visualization tracks how assessment accuracy changes over time for each major property type. Residential types generally remain below 1, indicating consistent undervaluation but relatively stable year-to-year patterns. However, some property types—especially commercial, public utility, and vacant land—show significant volatility, with sharp increases or decreases across certain years. These fluctuations can result from changes in market conditions, small sample sizes, or unique factors affecting specific property sectors. Understanding the long-term stability or instability of each property type’s assessment accuracy is critical for tax equity and municipal planning. Investors can also use this information to evaluate the reliability of assessed values for different property types. If a type shows increasing deviation from 1 over time, it signals that assessments are becoming less reflective of market trends, warranting further investigation.

# Snowflake Dashboard Links
Dashboard 1: https://app.snowflake.com/us-east-1/lec68149/#/2nd_question-d9aiRM17n
Dashboard 2: https://app.snowflake.com/us-east-1/lec68149/#/project-2-mist-4610-dIKu2WlXo

# Conclusion
Overall, our findings show which types of properties sell the most, which property types and towns are closest to or farthest from their assessed values, and how assessment accuracy changes over time. By analyzing trends in sale amounts, assessed values, property types, and sales ratios, our team was able to draw clear connections to our two main research questions and uncover meaningful insights about Connecticut’s real estate market.

Our first research question asked how towns’ median assessed and sale values compare to the statewide medians across different years and which towns consistently rank above or below statewide trends. Through our SQL queries that calculated town-level medians, value differences, and yearly sale trends, our visualizations clearly showed that towns such as Greenwich, Darien, and New Canaan consistently outperform the statewide median in both assessed and sale values. The heatgrid revealed long-term upward trends in these markets, highlighting their continuous growth and desirability. Conversely, more affordable towns consistently fell below statewide medians, reinforcing patterns of geographic inequality and variation in housing demand across Connecticut. Our queries enabled us to calculate year-over-year medians quickly and compare towns directly to statewide baselines, allowing us to visualize how property values diverged or aligned with statewide patterns.

Our second research question asked which property types sell closest to their assessed values, which types are over- or under-assessed, and how valuation accuracy varies across towns and over time. Using our calculated sales ratio field (sr_dec), supported by SQL queries grouped by property type, town, and year, we discovered clear patterns of undervaluation—especially in residential categories—and volatility in certain nonresidential types like commercial and public utility properties. The heatgrid of town-year sales ratios allowed us to identify towns with persistent undervaluation, while the scatter plot comparing median assessed vs. sale values helped us pinpoint towns whose assessments are closely aligned with or significantly lag behind market values. Our queries made it possible to compute median ratios efficiently and evaluate which property types consistently sold above their assessed values, highlighting where reassessment efforts may be most necessary.

Together, the dashboards tied to our SQL queries provided a comprehensive view of Connecticut’s real estate market. By cleaning our dataset, creating meaningful calculated fields, and using Snowflake to execute precise analytical queries, we were able to uncover clear trends in market performance, valuation accuracy, and property type behavior. These findings help municipalities identify areas where assessments need to be updated, assist investors in recognizing undervalued or high-growth markets, and offer insight into how local economic conditions influence housing demand and property valuation. Our project demonstrates how SQL-driven analysis and visualization can directly answer complex research questions and provide actionable insights for real-world decision-making.


