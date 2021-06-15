# zillow_regression_project

## This is the README for the Zillow Regression Project

### Building a Predictive Model for Property Values in Los Angeles County, Orange County and Ventura County, CA

### Goals
- Goal 1: Predict the values of single unit properties based on transactions dates between May - August 2017 
- Goal 2: Identify the county and state where the properties are located in addition to the distribution of property tax rates.

### Hypotheses and Questions
- Is there a correlation between number of bathrooms and tax appraised value?
- If there a correlation between number of bedrooms and tax appraised value?

### Included in this repo:


- This Readme file:

    - Project Overview and Key Takeaways
    - Data Dictionary
    - Skills and tools necessary for replication
    - Outline of process and tips for replication
    
- Python files needed:

    - acquire.py
    - wrangle_zillow.py
    - evaluate.py
    
- Final notebook with:

    - Explanation of acquiring, cleaning and prepping the data
    - Exploratory analysis
    - Hypotheses
    - Visualizations
    - Baseline model creation
    - Final model development
    
- My Google slide presentation is located [here](https://docs.google.com/presentation/d/1uHzSAQO84bC6w9ilzks5Rrr1gbrDY3NbPW4_s5zKI90/edit?usp=sharing)

### Data Dictionary
| Target            | Description                                | Data Type |
|--------------------|--------------------------------------------|-----------|
| taxvaluedollarrcnt | The total tax assessed value of the parcel | float64   |



| Attribute                    | Definition                                                                                                         | Data Type |
|------------------------------|--------------------------------------------------------------------------------------------------------------------|-----------|
| parcelid                     | Unique identifier for each property                                                                                | int64     |
| bathroomcnt                  | Count of number of bathrooms                                                                                       | float64   |
| bedroomcnt                   | Count of number of bedrooms                                                                                        | float64   |
| calculatedfinishedsquarefeet | Calculated total finished living area of the property                                                              | float64   |
| fips                         | Federal Information Processing Standard code - see https://en.wikipedia.org/wiki/FIPS_county_code for more details | int64     |
| tax_rate                     | Calculated tax rate for the property                                                                               | float64   |
| taxamount                    | The total property tax assessed for that assessment year                                                           | int64     |
| propertylandusetypeid        | Type of land use the property is zoned for                                                                         | int64     |


### Tips for Project Replication

#### Technical Skills

- Python:

    - Pandas
    - Seaborn
    - Matplotlib
    - Numpy
    - Sklearn 
- SQL

- Statistical Analysis:

    - Descriptive Stats
    - Hypothesis Testing
    - Pearsons Correlation Testing
    - Independent T-test
    
- Regression Modeling:

- Linear Regression:

    - LASSO + LARS
    - Generalized Linear Model (TweedieRegressor)
    - Baseline Accuracy
    
#### Project Process

Trello Board: [here](https://trello.com/b/Upj8GXV8/zillow-regression-project)
Key Findings:

- Number of Bathrooms, Number of Bedrooms, and Finished Living Area Square Feet are the top three drivers of property value.
- The mean baseline is $442223.20 and the baseline model performance can be evaluated by an RMSE of $417210.06
- The GLM model performs better than the baseline model with a RMSE of $356,139.80 on out of sample data.
