# About Dataset
This is the dataset used in the second chapter of Aurélien Géron's recent book 'Hands-On Machine learning with Scikit-Learn and TensorFlow'. It serves as an excellent introduction to implementing machine learning algorithms because it requires rudimentary data cleaning, has an easily understandable list of variables and sits at an optimal size between being to toyish and too cumbersome.  

**1. longitude:** A measure of how far west a house is; a higher value is farther west  
**2. latitude:** A measure of how far north a house is; a higher value is farther north  
**3. housingMedianAge:** Median age of a house within a block; a lower number is a newer building  
**4. totalRooms:** Total number of rooms within a block  
**5. totalBedrooms:** Total number of bedrooms within a block  
**6. population:** Total number of people residing within a block  
**7. households:** Total number of households, a group of people residing within a home unit, for a block  
**8. medianIncome:** Median income for households within a block of houses (measured in tens of thousands of US Dollars)  
**9. medianHouseValue:** Median house value for households within a block (measured in US Dollars)  
**10. oceanProximity:** Location of the house w.r.t ocean/sea  

The target variable in this dataset is median_house_value (price of houses).  
The goal is to predict a continuous numeric value (house price) from input features such as income, location, rooms, population, etc.
