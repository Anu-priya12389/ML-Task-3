# Large-Scale Geographic Consumer Clustering & High-Dimensional Visualizations

## Project Overview

This project analyzes large-scale real-estate transaction data using geographic coordinates and multiple property features. Machine learning clustering techniques are used to identify distinct housing market segments, which are visualized through interactive geographical maps.

The project is implemented using Python and Google Colab, with Folium used for interactive geographic visualization.

---

## Objectives

- Analyze large-scale real-estate transaction data
- Use latitude and longitude for geographic analysis
- Apply feature scaling to multivariate property data
- Perform unsupervised machine learning using K-Means clustering
- Identify distinct real-estate market segments
- Visualize property clusters geographically
- Create interactive map layers for business expansion analysis
- Analyze property density using heatmaps

---

## Dataset

The project uses the King County House Sales Dataset.

### Dataset Size

- 21,613 real-estate transactions
- 21 features

### Important Features

- Price
- Bedrooms
- Bathrooms
- Living Area
- Lot Area
- Floors
- Condition
- Grade
- Year Built
- Latitude
- Longitude

---

## Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Scikit-learn
- Folium
- Matplotlib

---

## Methodology

### 1. Data Ingestion

The real-estate transaction dataset was loaded into a Pandas DataFrame.

### 2. Data Preprocessing

- Checked missing values
- Verified data types
- Converted the date column to datetime format
- Validated latitude and longitude values

### 3. Feature Selection

Multiple property and geographic features were selected for clustering, including:

- Latitude
- Longitude
- Price
- Bedrooms
- Bathrooms
- Square footage
- Property condition
- Property grade
- Year built

### 4. Feature Scaling

StandardScaler was used to normalize the features so that variables with larger numerical values would not dominate the clustering algorithm.

### 5. Clustering

K-Means clustering was applied to segment properties into five distinct market clusters.

### 6. Market Segmentation

The clusters were interpreted based on average property characteristics.

| Cluster | Market Segment |
|---|---|
| Cluster 0 | Premium Large-Lot Market |
| Cluster 1 | Modern Mid-Market |
| Cluster 2 | Luxury Market |
| Cluster 3 | Affordable Entry-Level Market |
| Cluster 4 | Established High-Value Market |

---

## Interactive Geographic Visualization

Folium was used to create interactive maps displaying:

- Real-estate property locations
- Color-coded market segments
- Property information popups
- Interactive market segment layers
- Geographic property density heatmaps

Users can enable or disable individual market segments using the interactive layer control.

---

## Visualizations

The project includes:

1. Interactive real-estate property map
2. Marker clustering visualization
3. Color-coded market segmentation map
4. Interactive geographical layers
5. Property density heatmap
6. Geographic cluster distribution chart
7. Elbow Method visualization for selecting K

---

## Business Applications

The identified market segments can support:

- Corporate expansion planning
- Real-estate investment analysis
- Housing market analysis
- Location-based business strategy
- Identification of premium and affordable markets
- Geographic consumer segmentation

---

## Project Workflow

Dataset
↓
Data Preprocessing
↓
Geographic Coordinate Validation
↓
Feature Selection
↓
Feature Scaling
↓
K-Means Clustering
↓
Market Segmentation
↓
Interactive Folium Maps
↓
Business Insights

---

## Output

The final output is an interactive HTML map:

`real_estate_market_segmentation_map.html`

The map allows users to explore real-estate properties and their corresponding market segments geographically.

---

## Conclusion

This project demonstrates how machine learning and geospatial visualization can be combined to analyze large-scale real-estate transaction data. K-Means clustering identifies meaningful housing market segments, while Folium provides an interactive geographic interface for exploring these segments.

The resulting system can support data-driven real-estate analysis and corporate expansion planning.
