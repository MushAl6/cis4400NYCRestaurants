# cis4400NYCRestaurants
Analysis of NYC restaurant inspections and Yelp ratings, with data sourced from NYC Open Data and Yelp API, to explore the correlation between health violations and customer reviews.

## Table of Contents
- [Project Overview](#project-overview)
- [Information Architecture](#information-architecture)



## Project Overview
This project analyzes the correlation between NYC restaurant health violations and Yelp ratings. By combining health inspection data from NYC Open Data with Yelp customer reviews, the project provides actionable insights for:
- Restaurant owners to improve compliance and customer satisfaction.
- Health inspectors to identify borough-wide trends and recurring violations.
- Policymakers to create regulations that improve public health and safety.


## Information Architecture
The Information Architecture describes the data flow and tools used in the project pipeline:

1. **Data Sources**:
   - NYC Open Data:
     - [DOHMH New York City Restaurant Inspection Results](https://data.cityofnewyork.us/Health/DOHMH-New-York-City-Restaurant-Inspection-Results/43nn-pn8j/about_data)
     - [Open Restaurants Inspections](https://data.cityofnewyork.us/Transportation/Open-Restaurants-Inspections/4dx7-axux/about_data)
   - Yelp Dataset and API:
      - [Yelp Dataset](https://www.yelp.com/dataset)
      - [Yelp Fusion API](https://docs.developer.yelp.com/)
      - Provides restaurant ratings, review counts, and metadata.

2. **Pipeline Stages**:
- **Data Collection**: Collect data from NYC Open Data and Yelp APIs.
- **Cleaning**: Handle missing values, duplicates, and align data formats.
- **Transformation**: Reformat data into a star schema for analysis.
- **Storage**: Store intermediate data in MongoDB and processed data in Azure.
- **Visualization**: Create dashboards in Tableau to present insights.

3. **Key Tools**:
   - Data collection via APIs.
   - MongoDB for raw data storage.
   - Google Colab and Microsoft Azure for data processing and storage.
   - Tableau for visualization.
