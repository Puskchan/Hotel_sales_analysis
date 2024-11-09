---

# Hospitality Dashboard

In this end-to-end data analytics project, we focus on AtliQ Grands' hospitality data. The company is facing a decline in market share and revenue in the luxury/business hotels category due to competition and poor management decisions. This dashboard provides a comprehensive view of key metrics for the company, allowing business to monitor performance and make data-driven decisions to enhance operations, improve guest satisfaction, and optimize revenue.

![image](https://github.com/user-attachments/assets/445b1d06-dac9-46fd-a801-0c05f9a633c3)


## 📈 Dashboard Overview

This dashboard is designed to track and analyze data across various aspects of hospitality management, including room occupancy, revenue generation, customer satisfaction, and operational efficiency. By centralizing these key metrics, the dashboard enables quick insights that can help identify trends, assess business health, and pinpoint areas for improvement.

## 🖥️ Key Features

- **Room Occupancy Analysis**: Visualize occupancy rates across different time frames to understand seasonal or weekly trends.
- **Revenue Insights**: Analyze revenue from room bookings, food and beverage services, and other amenities, allowing for an understanding of the most profitable segments.
- **Customer Feedback & Satisfaction**: Track customer reviews and satisfaction scores to gauge the guest experience and identify areas to enhance service.
- **Cost Management**: Monitor operational expenses, including housekeeping, utilities, and staffing, to ensure efficient resource allocation.
- **Marketing and Sales Performance**: Evaluate the performance of marketing campaigns, referral programs, and other sales initiatives.

## 🚀 Business Insights and Actionable Steps

### 1. Optimize Room Occupancy Rates
   - **Insight**: By tracking occupancy trends, you can identify peak and off-peak periods.
   - **Actionable Step**: Offer promotions during off-peak times or increase rates during high-demand periods to maximize revenue.

### 2. Improve Customer Satisfaction
   - **Insight**: Consistent feedback analysis helps spot patterns in guest satisfaction or dissatisfaction.
   - **Actionable Step**: Address frequently mentioned issues (e.g., room cleanliness, food quality) to enhance guest experience and increase repeat bookings.

### 3. Increase Revenue Streams
   - **Insight**: Monitoring revenue across different services (rooms, dining, spa, etc.) reveals the most profitable offerings.
   - **Actionable Step**: Invest in high-performing areas or consider cross-promotions (e.g., bundling spa services with room packages) to increase spend per guest.

### 4. Control Operational Costs
   - **Insight**: Identifying high-cost areas (e.g., utilities, housekeeping) helps in optimizing resource allocation.
   - **Actionable Step**: Implement energy-saving practices or efficient staffing models to reduce operational expenses.

### 5. Boost Marketing Effectiveness
   - **Insight**: Track conversion rates of marketing efforts to assess return on investment (ROI).
   - **Actionable Step**: Focus on high-converting channels or reallocate budget from underperforming campaigns.

## 🛠️ Tech Stack

- **Tool**: Microsoft Power BI
- **Database**: Data sources include (add specific sources if known, e.g., SQL databases, CSV files, API integration for real-time data)
- **Data Processing**: Aggregation, transformation, and visualization are done through Power BI’s DAX functions and Power Query Editor.

## 📊 Usage Instructions

1. **Clone this Repository**: Clone the repository using the following command:
   ```bash
   git clone https://github.com/yourusername/hospitality-dashboard.git
   ```
2. **Open the Dashboard**: Open the Power BI file (`hospitality_dashboard.pbix`) in Power BI Desktop.
3. **Connect to Data Sources**: Update data source paths if necessary, and refresh the data model to load the latest information.
4. **Customize Filters**: Adjust filters on the dashboard to explore different segments, time frames, or departments.

## 🛢 Data Schema

The 5 CSV files out of which this dashboard has been created:
1. dim_date
2. dim_hotels
3. dim_rooms
4. fact_aggregated_bookings
5. fact_bookings


Column Description for dim_date:
1. `date`: This column represents the dates present in May, June and July.
2. `mmm yy`: This column represents the date in the format of mmm yy (monthname year).
3. `week no`: This column represents the unique week number for that particular date.
4. `day_type`: This column represents whether the given day is Weekend or Weekeday.



Column Description for dim_hotels:
1. `property_id`: This column represents the Unique ID for each of the hotels.
2. `property_name`: This column represents the name of each hotel.
3. `category`: This column determines which class[Luxury, Business] a particular hotel/property belongs to. 
4. `city`: This column represents where the particular hotel/property resides in.



Column Description for dim_rooms:
1. `room_id`: This column represents the type of room[RT1, RT2, RT3, RT4] in a hotel.
2. `room_class`: This column represents to which class[Standard, Elite, Premium, Presidential] particular room type belongs.


Column Description for fact_aggregated_bookings:
1. `property_id`: This column represents the Unique ID for each of the hotels.
2. `check_in_date`: This column represents all the check_in_dates of the customers.
3. `room_category`: This column represents the type of room[RT1, RT2, RT3, RT4] in a hotel.
4. `successful_bookings`: This column represents all the successful room bookings that happen for a particular room type in that hotel on that particular date.
5. `capacity`: This column represents the maximum count of rooms available for a particular room type in that hotel on that particular date.



Column Description for fact_bookings:
1. `booking_id`: This column represents the Unique Booking ID for each customer when they booked their rooms.
2. `property_id`: This column represents the Unique ID for each of the hotels
3. `booking_date`: This column represents the date on which the customer booked their rooms.
4. `check_in_date`: This column represents the date on which the customer check-in(entered) at the hotel.
5. `check_out_date`: This column represents the date on which the customer check-out(left) of the hotel.
6. `no_guests`: This column represents the number of guests who stayed in a particular room in that hotel.
7. `room_category`: This column represents the type of room[RT1, RT2, RT3, RT4] in a hotel.
8. `booking_platform`: This column represents in which way the customer booked his room.
9. `ratings_given`: This column represents the ratings given by the customer for hotel services.
10. `booking_status`: This column represents whether the customer cancelled his booking[Cancelled], successfully stayed in the hotel[Checked Out] or booked his room but not stayed in the hotel[No show].
11. `revenue_generated`: This column represents the amount of money generated by the hotel from a particular customer.
12. `revenue_realized`: This column represents the final amount of money that goes to the hotel based on booking status. If the booking status is cancelled, then 40% of the revenue generated is deducted and the remaining is refunded to the customer. If the booking status is Checked Out/No show, then full revenue generated will goes to hotels.

---

