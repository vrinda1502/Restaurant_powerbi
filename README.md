# Restaurant_powerbi

Problem Statement: To identify the restaurant in Mexico, which is highly rated and also to identify the restaurant for the future investments. Also, analyze the consumer preferences and demographics effect.

About Data: The dataset is from 2012 real consumers, available at Restaurant Ratings Dataset. It contains 5 csv files : consumer_preferences, consumers, ratings, restaurants_cuisines, restaurants.

Before making a visualization using the data in powerBI, we will follow certain steps as mentioned below:

Data Loading and Cleaning: This is the first step of getting started with powerBI here we connect the data source (i.e. csv files) and load them to power query editor, which is basically data transformation editor. Here, we can perform many task such as modify data type, remove or replace null and duplicate values, create, delete, merge, rename columns. In consumer table we have many blank cells in smoker, drink_level, transportation_method, marital_status, children, occupation etc. which is replaced by "NA".

Data Relationship Modeling: This is the second and crucial step for data analysis, in this step we make connection between the tables following one to many relationship. Here consumers and restaurants table having distinct primary key only are kept on one side and others tables on many side. (see fig.)

<img width="554" alt="image" src="https://user-images.githubusercontent.com/44741582/211062347-97eb6738-586e-46d5-b9ef-a32589b77c79.png">

Creating Calculated Columns and Explicit Measures using DAX: In data analysis we will make a use of very powerful Data Analysis Expression language. We can create new metrics and columns to gain more valuable insights from our data and drill down to more specific level. We have created calculated columns such as cuisines ordered in consumers table and order taken in restaurants table, also created measures like total restaurants, total cuisines, highly satisfied consumers/restaurants etc.


Report and Visualization: This is the final step where we develop charts and graphs. We have created multiple reports by restaurants, by cuisines, by ratings, by consumers also created restaurant report dashboard.

Inference:

Top City: From Restaurants report we can see that total restaurants are 130 of which 84 are from San Luis Potosi city. Similarly, from consumer report we can see out of 138 consumers same city has the highest of 86 consumers, again if we look with respect to orders as shown in cuisine report the San Luis Potosi has the highest orders 857 out of 1161 total orders. Thus, we can say that San Luis Potosi has the major impact in restaurant business in Mexico.

Top Cuisine: The Mexican cuisine is the top most among the consumers as well as it is ordered maximum by restaurants as well.

Consumer Type: The maximum consumers are of age group 20-25, i.e. maximum are of students category. Nearly, 90% are single having medium budget size. One more interesting fact is that parking is good for the restaurants but maximum customers type are those who used public transport. Hence, restaurants must be reachable by public transport system. Also, Smoking and Drink level does not make much impact because non smokers are 79% and social plus casual drinker are 62%.

Top Restaurant: The top 3 restaurants received highest orders are Tortas Locas Hipocampo (36), Puesto De Tacos (32), Cafeteria Y Restaurant El Pacifico (28) based in a Sant Luis Potosi.

Restaurant Ratings: The top restaurant by orders received is also the top overall highly satisfied restaurant. The satisfaction rating also suggests that non smoking, medium pricing and no alcohol based restaurants are in large numbers. Thus, we can say that satisfaction rate driven by the quality of food and service.

Conclusion:

Tortas Locas Hipocampo is the top restaurant and the consumer oriented city is Sant Luis Patosi. The challenge in this would be that it will have high competition as well.
