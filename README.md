# British Airways Predicting Customer Buying Behavior

![British Airways](https://github.com/SreelakshmiRaurora/British_Airways_ML-project2/blob/main/istockphoto-1264345178-612x612.jpg)

## Project Objective
To proactively identify customers with a high probability of completing a booking,enabling targeted marketing and reducing boking abandonment.

## The Dataset: A first look
The dataset contains 50000 booking sessions with 14 features,includig:
- num_passengers
- purchaselead
- length_of_stay
- wants_preferred_seat
- Ad our target:booking_complete

## Key challenge: Data imbalance
A significant finding from the EDA is the severe imbalance in our target variable,'booking_complete'.

##Data Preparation strategy
 -Encoding
 -Scaling
 -Balancing

## Key Predictive features
The correlation matrix revealed strong indicators of bookingintent.
-High intent:'wants_extra_baggage' , 'wants_preferred_seat' , 'wants_in_flight_meals'.
-Negative Factor: 'purchase_lead'.The further in advance a customer looks, the less likely they are to book in thatsession.
This tells us that customers who select ancilary products are signaling a strong intent to buy.

## K-Nearest Neighbours
   A non-linear model was chosen to capture more complex relationships in the data.

## Hyperparameter Tuning with RandomiszedSearchCV
   -Tuning
   -Validation
   -Scoring

## KNN performance (cross-validation)
0.8501
Promising Results
The 'RandomizedSearchCV' yielded a strong mean score of 85%.

## The test set: A critical insight
However, when the final KNN model was applied to the unseen test set, the confuion matrix revealed a critical problem.

