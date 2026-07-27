# Large-Scale Geographic Consumer Clustering & High-Dimensional Visualizations

## Project Overview

This project analyzes real-estate properties in Chennai, Tamil Nadu using machine learning and geospatial visualization techniques.

The project uses K-Means clustering to automatically segment properties into distinct housing market groups based on property characteristics, price, quality, and geographic location.

The resulting market segments are visualized using an interactive Folium map.

## Dataset

The project uses the Chennai Housing Sales Price dataset.

- 7,109 property records
- 22 original features
- 7 Chennai geographic areas

### Geographic Areas

- Karapakkam
- Anna Nagar
- Adyar
- Velachery
- Chrompet
- KK Nagar
- T Nagar

## Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Scikit-learn
- Folium
- Matplotlib

## Project Workflow

Dataset  
↓  
Data Loading  
↓  
Data Cleaning  
↓  
Area Name Standardization  
↓  
Geographic Coordinate Mapping  
↓  
Feature Selection  
↓  
Feature Scaling  
↓  
Elbow Method  
↓  
K-Means Clustering  
↓  
Market Segmentation  
↓  
Interactive Folium Map

## Data Preprocessing

The dataset was checked for missing values.

Missing values were found in:

- Number of bedrooms
- Number of bathrooms
- Overall quality score

These missing values were handled using median imputation.

Inconsistent area names were also standardized.

Examples:

- Karapakam → Karapakkam
- Ana Nagar → Anna Nagar
- Ann Nagar → Anna Nagar
- Adyr → Adyar
- Velchery → Velachery
- Chrompt → Chrompet
- Chrmpet → Chrompet
- Chormpet → Chrompet
- KKNagar → KK Nagar
- TNagar → T Nagar

## Geographic Analysis

The original dataset contained area names but did not include latitude and longitude coordinates.

Approximate geographic coordinates were assigned to each Chennai area to enable geographic visualization using Folium.

The geographic features used for analysis were:

- Latitude
- Longitude

These coordinates represent area-level locations and are not exact GPS coordinates for individual properties.

## Machine Learning Methodology

### Feature Selection

The following features were used for clustering:

- Property size (INT_SQFT)
- Distance from main road (DIST_MAINROAD)
- Number of bedrooms
- Number of bathrooms
- Number of rooms
- Room quality score
- Bathroom quality score
- Bedroom quality score
- Overall quality score
- Registration fee
- Sales price
- Latitude
- Longitude

### Feature Scaling

StandardScaler was used to standardize all numerical features before applying K-Means clustering.

This prevents features with larger numerical values, such as sales price, from dominating the clustering process.

### Clustering Algorithm

K-Means clustering was applied to divide the properties into four market segments.

The Elbow Method was used to determine the appropriate number of clusters.

## Market Segments

The four identified market segments are:

| Cluster | Market Segment |
|---|---|
| 0 | Compact Mid-Value Market |
| 1 | Large Family Market |
| 2 | Premium High-Value Market |
| 3 | Affordable Entry-Level Market |

## Interactive Map

An interactive geographical map was created using Folium.

The map provides:

- Chennai property locations
- Market segment visualization
- Interactive property popups
- Property information
- Separate layers for each market segment
- Layer control for turning market segments on and off

The final map output is:

chennai_real_estate_market_segments.html

## Business Applications

This project can support:

- Real-estate market segmentation
- Property investment analysis
- Geographic market analysis
- Corporate expansion planning
- Identification of premium housing markets
- Identification of affordable housing markets
- Location-based business strategy

## Key Findings

The clustering analysis identified four distinct housing market segments in Chennai based on:

- Property size
- Number of rooms
- Number of bedrooms
- Property quality
- Sales price
- Geographic location

The interactive Folium map allows users to explore the spatial distribution of these market segments.

## Project Output

The main output of this project is an interactive HTML map:

chennai_real_estate_market_segments.html

This map allows users to interactively explore different Chennai real-estate market segments.

## Conclusion

This project demonstrates how machine learning and geospatial visualization can be combined to analyze real-estate markets.

K-Means clustering was used to identify distinct housing market segments, while Folium was used to create an interactive geographical visualization.

The resulting system provides a data-driven approach for understanding Chennai's real-estate market and supporting geographic expansion and investment decisions.
