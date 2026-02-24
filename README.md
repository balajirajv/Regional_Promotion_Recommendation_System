# Project Title: Regional Promotion Recommendation System
## BTAA - Arizona State University

## Project Overview
This project builds a data-driven regional expansion strategy using 19 years of alcohol consumption data across 85 Russian regions.

The objective was to identify regions with consumption behavior similar to Saint Petersburg to optimize promotional investment and reduce expansion risk.

## Business Problem
Promotional campaigns were deployed without structured regional similarity analysis, resulting in:
 - High expansion uncertainty
 - Inefficient capital allocation
 - Poor regional targeting

To address this, we designed a multi-model recommendation system using clustering and similarity modeling to identify high-impact expansion regions.

## Dataset
- 19 Years of historical data
- 85 Russian regions (reduced to 81 after cleaning)
- 1,615 observations
- 7 Variables:
    - Year
    - Region
    - Wine
    - Beer
    - Vodka
    - Champagne
    - Brandy

Alcohol values represent per capita consumption (liters).

## Data Processing
- Removed 4 regions due to missing values
- Standardized per capita consumption metrics
- Enriched dataset with:
  - Latitude & Longitude
  - Regional geolocation classification
- Conducted time-series analysis (identified consumption dip in 2015)
- Performed correlation analysis
  - Champagne–Brandy correlation: 0.78

## Machine Learning Approach
To reduce model bias and improve robustness, multiple similarity techniques were applied:
 - Hierarchical Clustering
 - DBSCAN Clustering
 - Cosine Similarity
 - Collaborative Filtering (Euclidean Distance)

Regions were validated across all models to ensure recommendation consistency.

## Key Results
- Identified 3 regions consistently similar to Saint Petersburg:
   - Moscow
   - Khabarovsk Krai
   - Ivanovo Oblast
- Delivered Top 10 regional recommendation list
- Reduced expansion uncertainty through cross-model validation
- Created structured framework for scalable promotional expansion

## Business Impact
 - Enabled structured regional prioritization
 - Improved stakeholder confidence in promotional allocation decisions
 - Reduced over-processing by isolating relevant similarity clusters
 - Established scalable data-backed expansion strategy

## Tech Stack
 - Python
 - Pandas
 - NumPy
 - Scikit-learn
 - Matplotlib / Seaborn
 - DBSCAN
 - Hierarchical Clustering
 - Cosine Similarity
 - Power BI (Executive Dashboard)

## Repository Structure
data/

notebooks/

reports/

presentation/

## Future Improvements
 - Time-series forecasting (ARIMA / Prophet)
 - Uplift modeling for promotional impact measurement
 - ROI attribution tracking
 - Integration of demographic and economic indicators
 - API-based production deployment

## Team
DevilsBase - BTAA 2024

Arizona State University

## Contact
Balaji Raj Veluchamy
