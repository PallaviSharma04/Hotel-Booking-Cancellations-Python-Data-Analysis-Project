# Hotel Booking Cancellations (EDA Project) 

<img align="center" width="700" height="400" src="https://github.com/user-attachments/assets/43f499a2-c0ba-4183-8abf-412f4a4ba415">

## Table of Contents
- [Project Overview](#project-overview)
- [Project Goals](#project-goals)
- [Dataset](#dataset)
- [Tools & Technology](#tools-and-technology)
- [Analytical Approach](#analytical-approach)
- [Recommendations](#business-recommendations)

## Project Overview  
The City Hotel and Resort Hotel faces a significant challenge with booking cancellations in the year 2015-2017, affecting revenue, occupancy rates, and operational efficiency. This project analyzes booking data of the two hotels and explores patterns and trends in hotel booking cancellations through Exploratory Data Analysis (EDA). By analyzing key factors such as average daily rate(ADR), lead time, customer type, deposit policies, market segment and identifying patterns in cancellation trends we aim to uncover insights that can help hotels minimize cancellations ,optimize booking strategies and improve their revenue management and customer satisfaction strategies.  

## Project Goals
✅ Identify key factors affecting hotel booking cancellations.

✅ Analyze seasonal trends and customer behavior.

✅ Analyze how variables like deposit type, customer type, and ADR (Average Daily Rate) impact cancellations.

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

**2: Exploratory Data Analysis (EDA) and Insights**

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

> From the monthly ADR trends we observe that low ADR in August is driving higher bookings and lowest cancellations, hence it confirms that price sensitivity plays a significant role in customer decisions. Whereas the high cancellation rate in January suggests that customers might be making tentative bookings but canceling due to high prices. This could also indicate that travelers compare prices with competitors and opt for cheaper alternatives.

![ADR trends 2016-17](https://github.com/user-attachments/assets/2dc2ea2e-e77a-4609-8f57-a9caa9218025)

> Analyzing the relation between mean adr and reservation status indicates that canceled reservations have a higher ADR compared to confirmed reservations.The line graph further confirms our analysis that **the high cancellation rate is primarily driven by higher prices.**.


![Top 10 countries](https://github.com/user-attachments/assets/82f2d51b-8d18-4b51-8f50-238a715fc555)

> Now, let's identify the countries with the highest number of cancellations. The pie chart above displays the top 10 countries with the most cancellations.
**Portugal** accounts for the highest number of cancellations, making up 70% of the total cancellations.

![Cancellations by market segment](https://github.com/user-attachments/assets/961534f6-0419-49f5-ba03-cc4c3654391c)

> The pie chart reveals that **Online Travel Agencies(OTA)** bookings have the highest cancellation rates(**47%**). This can be due to the fact that customers on OTA platforms tend to compare multiple hotels and cancel frequently.

![Cancellations by deposit type](https://github.com/user-attachments/assets/2493a7fb-b8ca-482f-9324-27fb2e4f1fc3)

> Among all cancellations, the majority were from no deposit bookings (67%), followed by non-refundable bookings (32.79%), while refundable bookings had the least cancellations (0.08%).The high cancellation rate for no-deposit bookings suggests that customers may be making multiple reservations without a financial commitment, leading to last-minute cancellations.In contrast, non-refundable bookings still see cancellations but at a lower rate, indicating that some travelers are forced to cancel despite the financial penalty. Refundable bookings have the lowest cancellations, as travelers who choose this option are more likely to follow through with their stay.

![Cancellations by customer type](https://github.com/user-attachments/assets/7c4f7b8b-5c4a-4287-af4d-c1f8474c9a20)

> Individual(Transient) customers cancel the most, indicating they often book multiple options. Contracted customers and Group bookings have the lowest cancellation rates suggesting they are mostly commited once confirmed.

![Waiting and Cancellations](https://github.com/user-attachments/assets/a1b610ce-e6cd-4438-a9d5-f8f20b9df5ea)

> The strip plot analyzing waiting list days and cancellations shows no significant correlation between the two. This finding is unexpected, as it contradicts the common assumption that reservations left on the waiting list for extended periods are more likely to be canceled.

![Lead time and Cancellations](https://github.com/user-attachments/assets/e8d319f6-f103-402f-ba7d-76ddcac5a8eb)

> The strip plot analyzing lead time and cancellations reveals a weak to moderate positive correlation. This indicates that while cancellations tend to increase as lead time extends, the relationship is not particularly strong.

## Business Recommendations

Based on the Exploratory Data Analysis (EDA), the following strategies can help reduce cancellations and optimize revenue:

- **1. Pricing Strategies to Reduce Cancellations**: Higher ADR (Average Daily Rate) correlates with increased cancellations. Hotels should should adjust their pricing models that revises rates based on demand trends and seasonality. 
- **2. Addressing high cancellation in City Hotel**: City hotels observes a higher cancellation rate compared to Resort hotel. To attract more customers, they should offer discounts on extended stays that may encourage longer commitments, as well as early booking incentives to reduce last-minute cancellations.
- **3. Addressing Seasonal Cancellation Trends**: January sees the highest cancellations, while August has the lowest. Hotels should launch marketing campaigns in January to boost bookings (e.g., New Year promotions) also analyzing competitor rates in January can help set a more competitive ADR. Additionally they can implement stricter booking policies during peak months (August) to maximize revenue and limit no-shows.
- **4. Improve Quality of Services in Key Locations**: Since Portugal experiences a high cancellation rate, hotels in this region should enhance service quality, customer engagement, and brand trust to encourage more confirmed bookings.
- **5. Managing High-Risk Market Segments**: Group and OTA bookings show the highest cancellation rates. Hotels should require deposits or enforce stricter cancellation policies for Online bookings also encourage direct bookings by offering exclusive discounts or value-added perks (e.g., free breakfast, late check-outs).
- **6. Revising Deposit and Payment Policies**: Introducing a partial deposit policy instead of a fully no-deposit option may help lower cancellations while maintaining customer flexibility. Discounts or perks (e.g., free breakfast, room upgrades) for non-refundable bookings can encourage more secure reservations.

**Final Takeaway**:
> By adopting data-driven pricing, strengthening booking policies, and implementing targeted marketing strategies, hotels can effectively reduce cancellations, improve revenue, and enhance customer satisfaction.
