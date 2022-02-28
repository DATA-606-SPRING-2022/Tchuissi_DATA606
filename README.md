# Housing Price Prediction for Residential Properties in the DC area

# Introduction
Currently living in the DC area and passionate about real estate and construction, I want to analyze and understand the different criteria that define the selling price for residential properties.
The real estate market is every growing with properties more and more expensive.
The goal of this study is to identify the parameters that influence the selling price and map the area in DC with the most expensive houses.

# Unit of Analysis
My unit of analysis is housing in Washington DC at a city level and the unit type (houses).

# Hypothesis / Research Question(s)
- What are the attributes that affect the selling prices in DC downtown for houses?
- Are structural characteristics playing a role in the selling price?
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
- The second dataset is the adress residential units
- Number of rows: 272,531
- Number of columns: 8
- Web link: https://opendata.dc.gov/datasets/address-residential-units/explore

# Exploratory Data Analysis (EDA)

## EDA: General Statistics

![image](https://user-images.githubusercontent.com/70168968/155884650-797530ef-e449-46ce-9910-c463f3039872.png)

- Max selling price:
         $25,100,000
- Average selling price:
         $450,000
- Average bathrooms: 2
- Average bedrooms: 3
- Average stories: 2
- Average GBA: 1742 sqft

## EDA: Sales Frequency
### Year
![image](https://user-images.githubusercontent.com/70168968/155884737-69bcf267-6ac4-40c1-9bbc-5297c1438368.png)

- 2021,2020 and 2019 are the top years: More houses sold during the COVID-19
### Month
![image](https://user-images.githubusercontent.com/70168968/155884759-49ea4dc5-ba1d-4183-990e-91204c97f88f.png)

- More houses sold in January, July and June

## EDA: Variables Frequency 
### 1.Heat type
![image](https://user-images.githubusercontent.com/70168968/155884833-653eb12f-af4e-4519-82f3-969be6595162.png)
The three most common heat type are:
- Hot Water Rad (36.8%)
- Forced Air (35.8%)
- Warm Cool (25%)
### 2. House structure
![image](https://user-images.githubusercontent.com/70168968/155884851-97618645-afc7-41f6-afcc-8516c4a64a27.png)
The three most common house structures are:
- Row houses (50.6%)
- Single houses (29.4%)
- Semi-detached houses (15%)
### 3. Exterior Walls
![EXTWALLS](https://user-images.githubusercontent.com/70168968/155885002-ec15c11b-c2c9-4965-b4c6-609d25039d51.png)

The five common exterior walls are: 92056
- Common brick (75%)
- Brick/Siding (5.7%)
- Vinyl Siding (5.4%)
- Wood Siding (4.1%)
- Stucco (2.9%)
### 4. Interior walls
![INTWALL](https://user-images.githubusercontent.com/70168968/155885010-55e9684b-d14f-47be-b956-a1dd1c18c943.png)

The four common interior walls are:
- Hardwood (78.3%)
- Hardwood/carp (10.9%)
- Wood floor (7.1%)
- Carpet (3.3%)
### 5.Roof type
![roof](https://user-images.githubusercontent.com/70168968/155885097-649a17af-35d6-42f8-a093-ea1ef6c89521.png)

The four most common roof types are:

- Built up (29.7%)
- Comp Shingle (28.7%)
- Metal-sms (27.7%)
- Slate (10.1%)
### 6. Number of bathrooms
![BATHRM](https://user-images.githubusercontent.com/70168968/155885073-cc8a7517-a9f8-4d35-aa3d-7b86a81f6995.png)
Most of the houses have:

- 2 bathrooms (35.8%)
- 1 bathroom (30.6%)
- 3 bathrooms (22.4%)
- 4 bathrooms (8.8%)
### 7. Number of rooms
![ROOMS](https://user-images.githubusercontent.com/70168968/155885571-66d1ed37-9161-4695-a2e4-af02ad0030c0.png)

The most common rooms numbers are:

- 6 rooms (31.4%)
- 7 rooms (20.2%)
- 8 rooms (15.9%)
- 5 rooms (8.1%)
- 9 rooms (7.3%)
- 10 rooms (6%)
- 12 rooms (2.9%)
- 11 rooms (2.3%)
- 16 rooms (1.3%)
### 8. Number of bedrooms
![BEDRM](https://user-images.githubusercontent.com/70168968/155885643-4c2d720c-28a4-41f1-9a55-8bd132ac9dbb.png)
The most common rooms numbers are:

- 3 bedrooms (48.3%)
- 4 bedrooms (25%)
- 2 bedrooms (13.5%)
- 5 bedrooms (7.6%)
- 6 bedrooms (3.3%)

### 9. Number of stories
![STORIES](https://user-images.githubusercontent.com/70168968/155885655-3cb0cae5-295f-4fbd-9ecd-8eecebd71e44.png)

The most common stories numbers are:

- 2 stories (73.9%)
- 3 stories (9.4%)
- 2.5 stories (5.9%)
- 1 story (4.1%)
- 1.5 stories (2%)
## EDA: Correlation Matrix
![heatmap](https://user-images.githubusercontent.com/70168968/155885744-f9da5649-bed1-473e-890d-01fc80e2b46d.png)

The variables that are more correlated to the price are:
- Gross Building Area (GBA) (0.41)
- Number of bathrooms (0.42)
- Number of bedrooms (0.27)
- Number of rooms (0.24)
- Roof type (0.14)










# ML Techniques
- Split dataset
- Categorical data encoding
- Feature engineering
- Feature importance
- Feature selection with Random forest
- Training the models for continuous values: linear regression (Ridge, Lasso & Elastic Net), decision tree, random forest
- Accuracy methods (precision, recall, F1)
- Predict the housing prices on test dataset
- Visualization of the results
- Map of DC with prices

# Conclusion and lessons learned
