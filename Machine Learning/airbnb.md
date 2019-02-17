## [Search Ranking of Airbnb using Machine Learning](https://medium.com/airbnb-engineering/machine-learning-powered-search-ranking-of-airbnb-experiences-110b4b1a0789) 

- The main take-away is that machine learning-based Search Ranking works at every stage, given that we pick the model and infrastructure with the right level of complexity for the amount of data available and the size of the inventory that needs to be ranked
- Very complex models will not work well when trained with small amounts of data, and simple baselines are sub-optimal when large amounts of training data are available
### Stage 1: Build a Strong Baseline
 | Collecting training data | Labeling training data | Rank solely based on Experience Features | Training the ranking model - Gradient Boost Decision Tree | Testing the ranking model |
### Stage 2 : Personalize
| booked Airbnb Homes | user’s clicks | 
### Stage 3: Move to Online Scoring
| Model for logged-in users, which uses Experience Features, Query Features, and User (Personalization) Features |
Model for logged-out traffic, which uses Experience & Query Features, trained using data (clicks & bookings) of logged-in users but not considering Personalization Features | 
### Stage 4: Handle Business Rules

