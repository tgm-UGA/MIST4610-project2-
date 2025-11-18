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

