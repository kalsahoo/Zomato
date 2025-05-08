# Zomato Analysis
## project overview
Zomato is a restaurant search and discovery service. Operating in several countries worldwide, they provide detailed information and customer reviews of various restaurants. The owners of Zomato, want to unearth the hidden anomalies in their business data. The final objective is to analyze the data in a way which helps them to accurately judge their business performance.
## Data Sources
The data (sample) is currently available in the form of a few excel files with each file containing information about several restaurants operating in a specific continent. The clients want to create a consolidated and interactive PowerBI report from where they can easily analyze the following information:
Tools
-	Excel - Importing data
  [Download Here] (https://github.com/Simplilearn-Edu/Power-BI-Datasets.git)
- PowerBI - Creating Report
## Data Cleaning/Preparation
Data Transformations
1.	Some of the values in the “City” column, mentioned below, needs to be corrected. a. The word “city” needs to be taken off from every city name (wherever appears). b. “Sí£o Paulo” should be corrected to “São Paulo”. c. “Cedar Rapids/Iowa City” should be corrected to “Cedar Rapids”. d. “ÛÁstanbul” should be corrected to “Istanbul”.
2.	Remove the columns which are not used.
3.	Make separate columns to show the “Restaurant Name” and the “Restaurant Address”.
4.	Create a separate table from where you get the list of cuisines served by each restaurant.
5.	The “Country-Code” table must contain only unique and non-blank values (as it’s a dimension table).
Above transformations were done.

## Data Modeling
Country Code and Zomato Continents have one to many relationship. Zomato Continents and Cuisines have one to many relationship. Fact table and Zomato Continent have one to one relationship.
## Exploratory Data Analysis
### Using DAX
1. There needs to be a “Rating Color” column in an appropriate table. The data rows should follow the below mentioned convention.
Aggregate rating Rating color Above 4.5 Dark Green 4 to 4.4 Green 3.5 to 3.9 Yellow 2.5 to 3.4 Orange 1.8 to 2.4 Red 0 to 1.7 White
2.	Create following measures in appropriate tables. a. Restaurant Count b. Average Cost c. Average Rating d. Cuisine Count
### Data Visualization
Create the following visuals.
#### a. Card visual
- Average Cost
- Average Rating
- Restaurant Count
- selected restaurant’s address
#### b. Map visual
-	Geography hierarchy
-	Restaurant Count
#### c. Infographic designer
- Restaurant Name
- Top 5 Restaurants by Average Cost
- Average Rating
#### d. Slicer 
- showing list of rating colours
- showing list of countries
- showing list of cities
#### e. Grid 
- showing list of restaurants
- showing the selected restaurant’s list of cuisines
#### f. Gauge 
- showing selected restaurant’s average rating
- showing selected restaurant’s average cost

## Publish the report on to a service account and create a public link.

