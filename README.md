# travel-recommendation-system
## Travel destination recommender system implemented on real world data from Airbnb using XGBoost Classifier.

While we wait for the pandemic to pass, creating a recommendation system to help us find the best location for our adventure is an intriguing thought experiment with real-world
application. Airbnb is a website where users may reserve lodging while travelling. The challenge at hand is to forecast new users' initial booking destination. The users are all from the United States.
The dataset has 12 potential destinations: 'US','FR','CA','GB','ES','IT','PT','NL','DE','AU','NDF'(no destination found). Airbnb provided the dataset as part of a Kaggle competition in 2015. We used the XGBOOST machine learning approach to conduct a classification.

## We approached this project in 4 stages
### I. Data Exploration
The dataset contains 213451 rows and 16 columns.

#### a. Features given
• ID: User ID
• Date_account_created: the date of account creation
• Timestamp_first_active: Timestamp of the first activity, note that it can be earlier than date_account_created or date_first_booking because a user can search before signing up
• date_first_booking: date of the first booking
• Gender
• Age
• Signup_method: Airbnb website, Facebook, or Google
• Signup_flow: The page a user came to signup up from
• Language: International language preference
• Affiliate_channel: What kind of paid marketing
• Affiliate_provider: Where the marketing is e.g. google, craigslist, other
• First_affiliate_tracked: What the first marketing the user interacted with before signing up
• Signup_app : web based, mobile app base, etc.
• First_device_type: kind of device used.
• First_browser: what browser was used.
• Country_destination: This is the target variable to predict

#### b. Inference from visualization
● From 2010 to 2014, the date account created and the date first booking are exponentially increasing. However, we saw a decline in bookings from 2014 to 2015.
● There are more female travelers than male travelers. However, the majority of people do not reveal their gender.
● The average user is between the ages of 30 and 34. We have a large spike at 37 years of age, as expected.
● The majority of people use the website to find and access Airbnb. Users can also sign up for the website using Facebook.
● In the United States, the majority of users speak English.
● Chrome, Safari, and Firefox are the most popular browsers for accessing Airbnb.
● The most popular devices are Mac, Windows Desktop, and iPhone.
● The most popular trip destination is 'NDF.' Second, the majority of Americans travel within their own country. France, Canada, and England are three of the most popular overseas locations for Americans. They are, however, insignificant in relation to cross-country travel.

### II. Data preprocessing and EDA 
### III. Model implementation
Since our data was highly disorganised inspite of all the preprocessing and data handling, we noticed that the conventional ML models like Decision Trees or Random forests did not work on well and the prediction accuracy was very low. Hence we tried to use the data on more complex models in ML. We got beter results and accuracy rates for the XG Boost model due to which we based our recommendation system on Extreme Gradient Boosting Classifier for completing our task. 
### IV. Dstination prediction
Predicting top tourist destinations from the information given by Airbnb over the past few years of customer activity. 
