# Predicting-Food-Delivery-Time
### MachineHack Hackathon by IMS Proschool

Analytics India Magazine and IMS Proschool bring to you ‘Predicting Predicting Food Delivery Time Hackathon’.

Size of training set: 11,094 records

Size of test set: 2,774 records

### FEATURES:

Restaurant: A unique ID that represents a restaurant.

Location: The location of the restaurant.

Cuisines: The cuisines offered by the restaurant.

Average_Cost: The average cost for one person/order.

Minimum_Order: The minimum order amount.

Rating: Customer rating for the restaurant.

Votes: The total number of customer votes for the restaurant.

Reviews: The number of customer reviews for the restaurant.

Delivery_Time: The order delivery time of the restaurant. (Target Classes) 

### Data Observations and Processing
- From the above features we dropped the Restaurant and Location columns.
- There were a total of 101 cuisines with mutli-labelled values.
- We noticed that the 8 cuisines was the maximum number used to describe few of the rows, hence we introduced 8 columns to represent the cuisines.
- For rows which which had less than 8 cuisines the remaining values were stored as nan which we labelled as None.
- For newly opened resturants and resturants with blank we converted the value to 0.
- The data was also scaled.

### Training and Testing
In Final Predctions, we tired XGBoostClassifier and RandomForestClassifier but the accuracy wasn't very good on the test data.

Therefore, in Deep Learning, we used a neural network to predict the time taken for delivery.


