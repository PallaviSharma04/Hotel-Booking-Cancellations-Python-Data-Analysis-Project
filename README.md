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

**Data Source**: <a href ="https://github.com/PallaviSharma04/Hotel-Booking-Cancellations-Python-Data-Analysis-Project/blob/main/hotel_bookings.csv"> Dataset </a>

**Data Range**: July 2015 to Sep 2017

## Tools and Technology
This analysis was conducted using:

- **Python** for data processing and visualization.
- **Jupyter Notebook** for interactive data exploration.
- **Libraries Used**:
  - `Pandas` – Data manipulation and preprocessing.
  - `Matplotlib & Seaborn` – Data visualization.
 
## Analytical Approach

**1: Data Loading and Cleaning**

- The dataset was loaded into a Pandas DataFrame.
- The "reservation_status_date" column was converted to datetime format to facilitate time-based analysis.
- Unnecessary columns ("agent" and "company") were dropped due to excessive missing values.
- 488 rows with missing country data were removed.
- Outliers in ADR (negative values and extreme high values) were identified and filtered out.

**2: Exploratory Data Analysis (EDA)**

Key analysis and visualizations included:

![Reservation Status Count](https://github.com/user-attachments/assets/cf598307-f666-4b79-8e34-c36d52873d7a)

> The Bar graph shows that the overall cancellation rate is **37%** which means more than one-third of all bookings are cancelled. This is a high cancellation rate leading to revenue loss and insufficiencies in hotel operations.

![Hotel wise Reservation Status Comparison](https://github.com/user-attachments/assets/edcbc4ba-0dd8-4400-afb3-be2c3d4f248e)

> **City hotels** face a much higher cancellation rate (**42%**) compared to resort hotels (**28%**). Also the bookings in City hotel are more as compared to Resort hotels. It is possible that Resort hotels are more expensive than City hotels.

![Hotel wise ADR trends](https://github.com/user-attachments/assets/4ca74033-6cb2-4a00-83c4-9270c4ce6296)

> It can be observed from the line graph above that on most days the ADR for City hotel is lower that that of Resort hotel. **City hotel** have **lower price variability**, meaning more stable rates. **Resort hotel** have **higher ADR fluctuations**, likely due to seasonal pricing and peak vacation periods.

 
![Reservation Status per Month](https://github.com/user-attachments/assets/4214d552-e94d-44f6-a699-b13addf6b6b2)

> The grouped bar graph above shows the monthly reservation trends. It can be observed that the **highest number of confirmed reservations** as well as the **lowest cancellations** occur in the month of **August**. Whereas, **January** is the month with the **highest number of cancellations**. Could this variation in reservation status be influenced by pricing?

![Monthly ADR trends](https://github.com/user-attachments/assets/d82f86e0-3e0a-4826-8b83-ba43f5bc2990)

From the monthly ADR trends we observe that low ADR in August is driving higher bookings and lowest cancellations, hence it confirms that price sensitivity plays a significant role in customer decisions. Whereas the high cancellation rate in January suggests that customers might be making tentative bookings but canceling due to high prices. This could also indicate that travelers compare prices with competitors and opt for cheaper alternatives.

![ADR trends 2016-17](https://github.com/user-attachments/assets/2dc2ea2e-e77a-4609-8f57-a9caa9218025)

> Analyzing the relation between mean adr and reservation status indicates that canceled reservations have a higher ADR compared to confirmed reservations.The line graph further confirms our analysis that higher rate of cancellation is mainly due to higher prices.
> Now, let's identify the countries with the highest number of cancellations. The pie chart below displays the top 10 countries with the most cancellations.

![Top 10 countries](https://github.com/user-attachments/assets/82f2d51b-8d18-4b51-8f50-238a715fc555)

Portugal accounts for the highest number of cancellations, making up 70% of the total cancellations.
