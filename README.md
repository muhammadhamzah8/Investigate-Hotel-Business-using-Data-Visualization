# Investigate-Hotel-Business-using-Data-Visualization
Investigating Hotel Business using Data Visualization Python

## Background Project 

It is very important for a company to always analyze its business performance. Business performance analysis could help in finding problems and then put in place strategies to solve the issues, so that the company can reach their optimal potential.
This time, I will explore more about hotel business to find some insights. My focus is to analyze customer behavior in making hotel reservations, and which factor has the impact of cancellation rate of the reservations. The results of the insights I found later will be presented through visualizations for better understanding.
The dataset that will be used today is a dummy data contains a single file which compares various booking information between two hotels in Indonesia: a city hotel and resort hotel!

## Data Preprocessing

- Handling Missing values
There are 4 columns with missing values : children, city, agent, and company. Missing values in city column will be imputed with ‘Unknow’. As for the rest will be imputed with 0.
- Drop duplicated 
Drop duplicated data like 33261 data
- Fix data types
Change data types from float to integer for children, agent, and company columns.
- Fix Incorrect values
Replace ‘Undefined’ form ‘meal’ column with ‘No Meal’ as they both have the same meaning.
- Remove unnecessary data
Remove all data with 0 guest and 0 night

## Monthly Hotel Booking Analysis Based on Hotel Type
![image](https://user-images.githubusercontent.com/77976107/174631698-7e36708f-87e1-4790-9080-bdd599dad32b.png)
- Both hotel have more guest during holiday season, and City Hotel have most guest than Resort Hotel
- May–June is the holiday season for most schools in Indonesia. Usually there are many families who would go on a family trip at that time. This explain why May-June got more Guest from both Hotel.
- City Hotel gets sharply decreasing in guest from August - September

## Impact Analysis of Stay Duration on Hotel Bookings Cancellation Rates
![image](https://user-images.githubusercontent.com/77976107/174631943-b57079d9-a090-4573-a2af-b330752a231b.png)
- The longer total night booked, the higher the percentage of being cancelled, also City hotel has more steeper trend compare to Resort hotel.
- We can see that there is a positive trend on Total Night and Cancelation Rate for both hotels, the hotels should apply a cancellation policy. The longer the total nights booked, the higher the cancellation fee.

## Impact Analysis of Lead Time on Hotel Bookings Cancellation Rate
![image](https://user-images.githubusercontent.com/77976107/174631829-31950b2a-428b-4d61-9b9c-229c41e75de0.png)
<br>Both resort and city hotel have the highest cancellation rate around 1 year lead time. The customers probably forgot they have booked a hotel if the lead time is too long. The hotel could give reminders for them so that they would not cancel reservation. Also, by applying cancellation policy on every reservation could helps the hotel to prevent this from happening.

## Summary 
- Both hotels have more guest during holiday season, and City Hotel have more guest than Resort Hotel. It could be an advantage for the both hotel if they increase the price during the holiday season.
- The longer total night booked, the higher the percentage of being cancelled, also City hotel has more steeper trend compare to Resort hotel.
- Positive trend on Total Night and Cancelation Rate for both hotels, the hotels should apply a cancellation policy. The longer the total nights booked, the higher the cancellation fee.
- The lowest booking cancellation rate is for bookings with a waiting time of less than 30 days and applies to both types of hotels. 
- Resort Hotels are quite stagnant with a (40%) cancellation rate, while City Hotels have a fairly high ratio (60%) when the waiting time is around 1 year.
- Both resort and city hotel have the highest cancellation rate around 1 year lead time. The customers probably forgot they have booked a hotel if the lead time is too long. The hotel could give reminders for them so that they would not cancel reservation. Also, by applying cancellation policy on every reservation could helps the hotel to prevent this from happening.
