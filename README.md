# Hotel Booking Cancellations (EDA Project) 

<img align="center" width="700" height="400" src="https://github.com/user-attachments/assets/43f499a2-c0ba-4183-8abf-412f4a4ba415">

## Table of Contents
- [Project Overview](#project-overview)
- [Project Goals](#project-goals)
- [Dataset](#dataset)
- [Tools & Technology](#tools-and-technology)
- [Analytical Approach](#analytical-approach)
- [Business Insights](#business-insights)
- [Recommendations](#business-recommendations)

## Project Overview  
The City Hotel and Resort Hotel faces a significant challenge with booking cancellations in the year 2015-2017, affecting revenue, occupancy rates, and operational efficiency. This project analyzes booking data of the two hotels and explores patterns and trends in hotel booking cancellations through Exploratory Data Analysis (EDA). By analyzing key factors such as average daily rate(ADR), lead time, customer type, deposit policies, market segment and identifying patterns in cancellation trends we aim to uncover insights that can help hotels minimize cancellations ,optimize booking strategies and improve their revenue management and customer satisfaction strategies.  

## Project Goals
✅ Identify key factors affecting hotel booking cancellations.

✅ Analyze seasonal trends and customer behavior.

✅ Analyze how variables like lead time, deposit type, customer type, and ADR (Average Daily Rate) impact cancellations.

✅ Compare cancellation trends across City Hotels and Resort Hotels.

✅ Provide actionable data-driven insights and recommendations to reduce cancellations.

## Dataset
Download the dataset for this project from the following link:

**Data Source**: <a href ="https://github.com/PallaviSharma04/Hotel-Booking-Cancellations-Python-Data-Analysis-Project/blob/main/Hotel%20Booking%20Data%20Analysis%20using%20Python%20.ipynb"> Dataset </a>

**Data Range**: July 2015 to Sep 2017

## Tools and Technology
This analysis was conducted using:

- **Python** for data processing and visualization.
- **Jupyter Notebook** for interactive data exploration.
- **Libraries Used**:
  - `Pandas` – Data manipulation and preprocessing.
  - `Matplotlib & Seaborn` – Data visualization.
 
## Analytical Project

**1: Data Loading and Cleaning**

- The dataset was loaded into a Pandas DataFrame.
- Unnecessary columns ("agent" and "company") were dropped due to excessive missing values.
- 488 rows with missing country data were removed.
- Outliers in ADR (negative values and extreme high values) were identified and filtered out.

**2: Exploratory Data Analysis (EDA)**
Key analysis and visualizations included:

- Reservation Trends: Monthly cancellation patterns to identify peak cancellation periods.
- Hotel-wise Cancellation Rates: Comparison of cancellations between City Hotels and Resort Hotels.
- Lead Time Impact: Analyzing how booking lead time affects cancellation likelihood.
- Market Segments & Customer Type: Identifying high-risk segments with frequent cancellations.
- Deposit Type Influence: Examining how different deposit policies impact cancellation rates.
- ADR Trends Over Time: Comparing ADR fluctuations between 2016 and September 2017 to identify pricing trends.

Some interesting code worked with :




