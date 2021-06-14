# zillow_regression_project

## This is the README for the Zillow Regression Project

### Goals
- Goal 1: Predict the values of single unit properties based on transactions dates between May - August 2017 
- Goal 2: Identify the county and state where the properties are located in addition to the distribution of property tax rates.

### Hypotheses and Questions
- Is there a correlation between number of bathrooms and tax appraised value?
- If there a correlation between number of bedrooms and tax appraised value?

### Data Dictionary
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
