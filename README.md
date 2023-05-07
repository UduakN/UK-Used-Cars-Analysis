# UK-Used-Cars-Analysis
![image](https://user-images.githubusercontent.com/128192166/236651758-65a560ee-3fbc-41a2-921f-9a0c6cf890de.png)

The aim of this analysis is to determine factors that will aid to predict how much a used car should be compared to the market and determine ideal selling period. To achieve this aim below business questions were asked:

•	What is the average price of each car models?

•	What is the age of the cars?

•	What is the price per Mileage?

•	What is the average price per model?

•	What is the trend of price over the years?

•	What is the correlation between the price and mileage of the cars?

•	What is the distribution of fuel types across the dataset?

•	What is most used fuel type and why?

•	How does the road tax impact the price of the car?

•	What is the trend of the mileage and price of the cars over the years?

# Data Overview

The dataset was downloaded from an open source Kaggle https://www.kaggle.com/datasets/adityadesai13/used-car-dataset-ford-and-mercedes, produced by ADITYA. It was a zip folder that contained 13 files, which were 11 cleaned files and 2 unclean files.  

![image](https://user-images.githubusercontent.com/128192166/236651875-505d335c-df4f-4c86-98ec-9980b4d52aae.png)

# Data Transformation and Combining

Before data was transformed, the uncleaned data were deleted to avoid duplicates as they already exist as clean data. The data were imported into power bi using the folder option and then transformed into power query.
Before the files were combined, the unwanted data properties were deleted.

![image](https://user-images.githubusercontent.com/128192166/236651920-3ff14d33-4e1b-4840-96b7-9384d11eb41b.png)
![image](https://user-images.githubusercontent.com/128192166/236651955-45e8d33d-a86d-4878-81b4-5af6bda20755.png)


![image](https://user-images.githubusercontent.com/128192166/236652046-1ec2d370-cb2f-490c-9498-15c2057c2b0a.png)



# Further Analysis

After data was combined, I loaded into power bi for further analysis and visualization. 
Below are steps I took to provide answers to the business questions:

•	I created a column to calculate the age of the car using the year of manufacture

Car Age = 2023 - 'UK Used cars'[year]

•	I created another column to calculate price per mileage

Price per Mileage = 'UK Used cars'[price] / 'UK Used cars'[mileage]

•	I calculated the average price per model using DAX function

Average Price per Model = CALCULATE(AVERAGE('UK Used cars'[price]),FILTER(ALLSELECTED('UK Used cars'),'UK Used cars'[model]=MAX('UK Used cars'[model])))


# Data Visualization

![image](https://user-images.githubusercontent.com/128192166/236652105-8fc3d142-1092-478a-a6e4-9e4ee446f747.png)

# Summary of Findings and conclusion

•	2019 is the year with the highest price. Which makes it the best year to sell and worst year to buy

•	The most common fuel type is petrol. Petrol comes first with 55.16%, other fuel types are diesel(41.62%), hybrid (2.97%)

•	The average price per model of petrol is cheaper compare to others. The petrol price influenced the demand and supply

•	Price and mileage are positively correlated, they move in tandem

•	G class model has the highest average price of 99,000, followed closely by R8 model with 98,000

•	The year 2019 attributed most to the total price of 38.5% while 2011 attributed the lowest of 0.18% 

•	The newer the car, the higher the price

•	The major factors that determines how much a used car should be sold are model, age, fuel type and mileage

Connect with me on Linkedin https://www.linkedin.com/in/uduak-njoku






