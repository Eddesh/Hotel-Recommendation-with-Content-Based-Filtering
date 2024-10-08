# Hotel-Recommendation_Data_Science_Club_Olympiad_Final

## Project Overview
This project develops a hotel recommendation system using content-based filtering, aiming to suggest hotels that best align with a user’s preferences. Several datasets, containing information on room prices, amenities, and hotel characteristics, were merged and processed to build the recommendation engine. Extensive data cleaning and preprocessing were necessary due to the initially disorganized structure of the CSV files.

### Dataset Description
The project integrates multiple datasets:
- Room Prices Dataset: Contains information on hotel room rates, booking status, discounts, and other related attributes.
- Hotel Details Dataset: Provides hotel-specific details, such as location, star rating, and property type.
- Min/Max Price Dataset: Includes data on the minimum and maximum price range for various hotels, which is useful for budget filtering.
Due to the presence of NULL values, significant preprocessing was conducted, including removing unnecessary columns and imputing missing values.

### Step 1: Data Preprocessing and Cleaning
Data cleaning included removing duplicate and irrelevant columns and imputing missing values for features like promoname and mealinclusiontype. Afterward, the datasets were merged on shared attributes, creating a comprehensive dataset for the recommendation system.

### Step 2: Feature Engineering
To represent hotel attributes, term frequency-inverse document frequency (TF-IDF) was applied to transform the textual data (e.g., room amenities and descriptions) into numerical vectors. These vectors help in measuring attribute similarity between hotels, forming the basis for content-based filtering.

### Step 3: Building the Recommendation System
Using the processed data, a content-based filtering approach was implemented. The system calculates the cosine similarity between the user’s preferences and hotel features, recommending the most relevant hotels. The recommendations are evaluated based on the Precision@K metric with K=5, indicating the relevance of the top-5 recommendations.

## Testing
The recommendation model was tested and evaluated using Precision@5. The metric demonstrated that the system could consistently deliver relevant hotel options within the top recommendations, achieving high precision in matching user preferences with hotel features.

## Authors
Davin Edbert Santoso Halim, Brandon Ritchie Yang, Steve Marcello Liem
