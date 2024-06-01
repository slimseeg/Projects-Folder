# Project  2 - Legacy Landmark Inc Portfolio Diversification

![Home and keys image](home-pic.jpg) 

### Problem Statement

**Business Context**:

In light of the volatile commercial real estate market conditions and  diminishing values in commercial real estate holdings, Legacy Landmark Inc is exploring avenues to diversify its portfolio and mitigate further losses. Recognizing the opportunity in the residential real estate sector, Legacy Landmark Inc wants to add residential holdings to their portfolio. As a Legacy Landmark data scientist, you are to analyze local real estate market data to determine what property features most influence the value of a property and its sale price and create a model that confirms your analysis.

---


### Data Dictionary:

|Feature|Type|Dataset|Description|
|---|---|---|---|
|**SalePrice**|*int*|Ames Iowa Housing| Sale price $$|
|**Overall Qual**|*int*|Ames Iowa Housing| Rates the overall material and finish of the house
|**Gr Liv Area**|*int*|Ames Iowa Housing|Above grade (ground) living area square feet|
|**Garage Cars**|*float*|Ames Iowa Housing|Size of garage in car capacity|
|**Total Bsmt SF**|*float*|Ames Iowa Housing|Total square feet of basement area|
|**1st Flr SF**|*int*|Ames Iowa Housing|First Floor square feet|
|**Year Built**|*int*|Ames Iowa Housing|Original construction date|
|**Year Remod/Add**|*int*|Ames Iowa Housing|Remodel date (same as construction date if no remodeling or additions)|
|**Full Bath**|*int*|Ames Iowa Housing|Full bathrooms above grade|
|**Mas Vnr Area**|*float*|Ames Iowa Housing|Masonry veneer area in square feet|
|**TotRms AbvGrd**|*int*|Ames Iowa Housing|Total rooms above grade (does not include bathrooms)|


#### Project Datasets
train.csv
test.csv
tanyassubmission.csv

---

### Executive Summary

#### Conclusion and Recommendations

**Conclusions**

After thorough evaluation of all the correlating features in the supplied Ames Iowa dataset, I was able to infer from this sample data that the top 6 features that contribute most to the sale price of a residential property are:

1) Overall Home Quality. This refers to the materials used and finishes on the home. The better quality the materials used in the home, the more the home outperforms the median sale price.

2) Above Ground Living Area. Homes with 2k-3k+ square feet outperform median home sales be $70k-170k.

3) Garage Car Capacity. The median sale price for residential units with 2 or more car space capacity  is 175k - 295K, which is beats the median sale price of the dataset.

4) Total Basement Square Feet. Most homes without a basement fall below the median home sale price. Residential units with robust sale prices, beating the median value by $2k - 100K+ have basements 1k sq. ft or bigger.

5) Year Built. It's clear from graphs and distribution of Year Built versus sale price that homes more than 20 years are far more likely to be sell for less than the median sale price. Even older homes with higher overall quality didn't have as high of sale prices and homes built in the last 20 years.

6) Full Baths. Residential properties with at least 2 or more full baths beat median residential home sale price by between $50k-150K. Whereas, homes with 1 or fewer full baths sit at or below the median sale price.

**Recommendations**
With the goal of diversifying Legacy Landmark LLC's portfolio in order to mitigate further losses in the volitile commercial real estate market by expanding into more profitable residential real estate markets, my recommendations are to add residential units that were build after 2000 and have high quality materials throughout the home. I also recommend minimum above grade square footage of 2k plus units with basements. You should also consider homes with at least a 2 car capacity and at least 2 full baths.  

**Further Research**
Now that we've narrowed down the features that add the most value to a residential unit. I recommend analyzing markets within the state and throughout the country
