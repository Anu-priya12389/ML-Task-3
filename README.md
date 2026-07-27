# Large-Scale Geographic Consumer Clustering & High-Dimensional Visualizations

## Project Overview

This project analyzes real-estate properties in Chennai, Tamil Nadu using machine learning and geospatial visualization techniques.

The project uses K-Means clustering to automatically segment properties into distinct housing market groups based on property characteristics, price, quality, and geographic location.

The resulting market segments are visualized using an interactive Folium map.

---

## Dataset

The project uses the Chennai Housing Sales Price dataset.

### Dataset Size

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

## Project Workflow

```text
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
