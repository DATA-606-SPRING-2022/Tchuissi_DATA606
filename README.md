# Housing Price Prediction for Residential Properties in the DC area

# Introduction
Currently living in the DC area and passionate about real estate and construction, I want to analyze and understand the different criteria that define the selling price for both  residential and condo properties.
The real estate market is every growing with properties more and more expensive.
The goal of this study is to identify the parameters that influence the selling price and map the area in DC with the most expensive houses/condos.

# Unit of Analysis
My unit of analysis is housing in Washington DC at a city level and the unit type (houses or condos).

# Hypothesis / Research Question(s)
- What are the attributes that affect the selling prices in DC downtown for both houses and condos?
- Are structural characteristics playing a role in the selling price?
- Compare the rising in price between houses and condos?
- Is there any pattern/reason as to why the housing selling prices are rising over the years? Is the COVID-19 increased the prices faster than before?
- Where are the areas in DC with the highest selling prices?

# Dataset
- The first dataset contains attribution on housing and structural characteristics for residential properties.
Computer Assisted Mass Appraisal (CAMA) database. 
- The dataset contains attribution on housing characteristics for residential properties, and was created as part of the DC Geographic Information System (DC GIS) for the D.C. Office of the Chief Technology Officer (OCTO) and participating D.C. government agencies.
- Number of rows: 108,197 
- Number of columns: 39
- Examples of attributes: #bathroom, #bedrooms, #kitchens, GBA (Gross building area), saledate, heat type, stories,external walls type, internal walls type,roof type, structure type 
- Web link: https://opendata.dc.gov/datasets/DCGIS::computer-assisted-mass-appraisal-residential/about
- The second dataset is the same as the first one but for condos
- Number of rows: 58,655
- Number of columns: 39
- Web link: https://opendata.dc.gov/datasets/computer-assisted-mass-appraisal-condominium/explore
- The third dataset is the adress residential units
- Number of rows: 272,531
- Number of columns: 8
- Web link: https://opendata.dc.gov/datasets/address-residential-units/explore

# Exploratory Data Analysis (EDA)

- Handling missing value
- Columns renaming
- Statistical analysis
- Correlation matrix

# ML Techniques
- Split dataset
- Categorical data encoding
- Feature engineering
- Feature importance
- Feature selection
- Training the models: linear regression (Ridge, Lasso & Elastic Net), decision tree, random forest
- Accuracy methods
- Predict the housing prices on test dataset
- Visualization of the results

# Conclusion and lessons learned
