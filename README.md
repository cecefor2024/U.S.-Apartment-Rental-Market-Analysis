# U.S.-Apartment-Rental-Market-Analysis
This project explores the UCI Apartment for Rent Classified Dataset to uncover what factors most strongly influence U.S. apartment rental prices. Conducted from the perspective of data analysts at StreetEasy, a real estate platform, the analysis investigates four research questions spanning physical apartment features, geographic location, bedroom count, and listing photography.

Dataset Source
UCI Machine Learning Repository — Apartment for Rent Classified (#555)
The dataset contains apartment rental listings aggregated from multiple U.S. online housing platforms.

Research Questions
RQ1: Square Footage & Price
RQ2: Geographic Location & Price
RQ3: Bedroom Count & Price (my section)
How much does the number of bedrooms affect listed price?
Methods: Data cleaning, OLS linear regression (statsmodels), residual plot analysis
Finding: The OLS regression found a statistically significant negative coefficient on bedroom count (F-statistic: 4.334, p = 0.037), though the R² of 0.001 indicates that bedrooms alone explain virtually none of the variation in price. The counterintuitive negative coefficient is likely driven by confounding variables (location, amenities) and extreme outliers in the dataset. Bedroom count is a weak standalone predictor; multiple regression with additional controls would produce more meaningful results.
RQ4 — Listing Photos & Price

Methods & Tools
Language: Python
Data Manipulation: pandas, numpy
Visualization: seaborn, matplotlib 
Statistical Modeling: statsmodels (OLS regression)
Machine Learning: scikit-learn (Random Forest Regressor/Classifier)
Geospatial: geopandas
Environment: Google Colab

Key Takeaways
Square footage is the strongest physical predictor of rental price among the features tested.
Location drives the most dramatic price variation; California and coastal metro areas command premium prices far above the national average.
Bedroom count alone is a poor predictor of price and requires additional covariates for meaningful modeling.
Listing photos are standard practice in the luxury market but have minimal impact on price in the general market; the real benefit of photos may be faster transaction speed rather than higher rent.

Authors
Gwendolyn Zawacki RQ1: Square Footage & Price
Amanda Vogel RQ2: Geographic Location & Price
Chelsea Oliveira RQ3: Bedroom Count & Price
Megan Lathrop RQ4: Listing Photos & Price
DIDA 325: Data, Information & Decision Analytics · Binghamton University
