# Hotel-Booking-Exploratory-Analysis
Capstone Project Exploratory Data Analysis on Hotel Booking

## Content

- ### Basic Information About Dataset

  - `hotel` :- Type of Hotel  ( City or Resort)
  - `is_canceled`	:- If booking of hotel is cancelled then 1 and if 0 then hotel is not cancelled
  - `lead_time`	:- Time (in days) between booking transaction and actual arrival.
  - `arrival_date_year`	:- Year of entry in the hotel 
  - `arrival_date_month` :- Month of entry in the hotel
  - `arrival_date_week_number`: Week Number of arrival date.
  - `arrival_date_day_of_month`: - Date of entry in the hotel corresponding to respective months
  - `stays_in_weekend_nights`:-  Number of weekends nights spent in a hotel
  - `stays_in_week_nights`	:- Number of week nights spent in a hotel
  - `adults`	:- Number of adults stayed in hotel
  - `children`:- Number of childrens stayed in hotel
  - `babies`:- Number of babies stayed in hotel
  - `meal`:- Type of meal chosen 
  - `country`:- Customers Country Origin
  - `market_segment`:- By which segment booking was made and for what purpose.
  - `distribution_channel`:- by which platform booking was made.
  - `is_repeated_guest`:- Whether the guest stayed preveously or not 
  - `previous_cancellations`:- No. of previous canceled bookings.
  - `previous_bookings_not_canceled`:- No. of previous non-canceled bookings.
  - `reserved_room_type`:-  Type of room reserved by a customer.
  - `assigned_room_type`:-  Type of room assigned to the customer.
  - `booking_changes`:- Number of booking changes done by customers
  - `deposit_type`:- Type of deposit at the time of making a booking (No deposit/ Refundable/ No refund)
  - `agent`:- Id of agent for booking
  - `company`:- Id of the company making a booking
  - `days_in_waiting_list`:- Number of days on waiting list.
  - `customer_type`:- Type of customer(Transient, Group, etc.)
  - `adr`:- Average Daily rate.
  - `required_car_parking_spaces`:- Number of car parking asked during booking
  - `total_of_special_requests`:- Total number of special request.
  - `reservation_status`:- Whether a customer has checked out or canceled,or not showed 
  - `reservation_status_date`:- Date of making reservation status.
      - Total Number of rows in datsets - 119390
      - Total Number of features presents - 32
- ### Data Cleaning
  - ### Removing Duplicates Values
      - All duplicates rows were droped
  - ### Handling Null Values
      - Replacing Null values present in column *`country`* with other(OTH)
      - Replacing null values present in column *`agent`* and *`company`* with 0
      - Replacing null values present in column *`children`* with mode value of that column ie. 0
  - ### Converting features into appropriate data type
      - Convert Data Type of features *`children`*, *`company`*, *`agent`* from float data type to integer data type.
      - Convert Data Type of feature *`reservation_status_date`* from object data type into DateTime data type.
