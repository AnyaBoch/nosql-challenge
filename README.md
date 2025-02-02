# nosql-challenge
## uk_food

The UK Food Standards Agency evaluates various establishments across the United Kingdom, and gives them a food hygiene rating. You've been contracted by the editors of a food magazine, Eat Safe, Love, to evaluate some of the ratings data in order to help their journalists and food critics decide where to focus future articles.

**Part 1: Database and Jupyter Notebook Set Up**

I created database **uk-food** and installed collection **establishments**
mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json

**Part 2: Update the Database**

I successfully updated collection with a new restaurant by the name "Penang Flavours" and updated its BusinessTypeID;
All the establishments within the Dover Local Authority were removed from the database;
Data types were checked and updated;

**Part 3: Exploratory Analysis**

##### The following questions to explore the database, and find the answers, so you can provide them to the magazine editors.
Which establishments have a hygiene score equal to 20?
There are 41 businesses in the area with such score.
First 10 Business Names are: 
The Chase Rest Home
Brenalwood
Melrose Hotel
Seaford Pizza
Golden Palace
Ashby's Butchers
South Sea Express Cuisine
Golden Palace
The Tulip Tree
F & S

##### Which establishments in London have a RatingValue greater than or equal to 4?
There are 33 establishments with a RatingValue of 4 or higher in the 'City of London Corporation. First 10 of them are:
Charlie's
Mv City Cruises Erasmus
Benfleet Motor Yacht Club
Coombs Catering t/a The Lock and Key
Tilbury Seafarers Centre
Mv Valulla
Tereza Joanne
Brick Lane Brews
WH Smith
City Bar & Grill

##### What are the top 5 establishments with a `RatingValue` rating value of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
Howe and Co Fish and Chips - Van 17
Lumbini Grocery Ltd T/A Al-Iman
Atlantic Fish Bar
Iceland
Volunteer

##### How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.

Number of establishments in the result: 55
Local Authorities with the highest number of establishments with hygiene score of 0, top 10:
'Thanet', 'count': 1130
'Greenwich', 'count': 882
'Maidstone', 'count': 713
'Newham', 'count': 711
'Swale', 'count': 686
'Chelmsford', 'count': 680
'Medway', 'count': 672
'Bexley', 'count': 607
'Southend-On-Sea', 'count': 586
'Tendring', 'count': 542
