# Executive Summary
The property market always fluctuates in differing ways, and the features that are important to sale price isn't always clear. From an extensive dataset over a period of 5 years, some data preparation, cleaning and exploratory analysis was done to obtain some insights into which factors affect house sale prices the most. A Lasso regression model with 37 variables and an R^2 value of 0.893 was obtained from the data analysed.

To no surprise, size of the living area, overall quality of the house and neighborhood ranked amongst the highest in how much price the house is able to fetch. However, there were a few surprising finds as well, such as lot area having low correlation with the sale price.

Some recommendations for owners to increase their sale price would include expanding their living area, remodeling of their house to increase overall quality.

# Problem Statement
Home sellers often anchor their offer price to avoid underselling, while home buyers, due to information asymmetry, often pay different prices for houses with similar features.

As a property consultancy firm, we aim to build a model to identify the features that are most important to predict sales price of houses. This would allow us to provide our clients with a tool that gives estimates of their potential selling prices and help them identify which aspects of their properties they can improve on to enhance their selling prices.

# Content
1. Initial Analysis & Data Inspection
2. Data Cleaning
3. Feature Engineering & Dimensionality Reduction
4. Regression Modeling

# Findings
Individual factors that most affected housing prices were:
1. Living Area Above Grade
2. Overall Quality
3. Neighbourhood - Northridge Height
4. Neighbourhood - Stone Brook
5. Basement Exposure

# Conclusions and Recommendations
How do you get an estimate of your house worth?
1. Living Area - Several other indoor related features such as full bathrooms and garage area also scored high.
2. Overall Quality - Don't skimp on materials! Quality of materials and finish matters.
3. Neighbourhood - Not all neighborhood are equal. Some such as Northridge Height boost the prices of houses whilst others like Edwards actually decreased the sale price.
4. House Age - Old is not gold. House prices tend to drop as they get older.
5. Building Type - If you have a townhouse, you're out of luck. Despite being the only 2 types that affected selling price, both were bad for sale prices whilst the rest were relatively unimportant.

To get a higher selling price, consider these:
1. Increasing your living area.
2. Remodel your house to improved quality and condition.

And lastly, anchor your expectations with your neighborhood or house type, as these are independent factors out of your control.

|Feature|Type|Dataset|Description|
|---|---|---|---|
|**mssubclass**|*object*|train_cleaned.csv|Identifies the type of dwelling involved in the sale.|
|**mszoning**|*object*|train_cleaned.csv|Identifies the general zoning classification of the sale.|
|**lotshape**|*object*|train_cleaned.csv|General shape of property.|
|**lotconfig**|*object*|train_cleaned.csv|Lot configuration.|
|**neighborhood**|*object*|train_cleaned.csv|Physical locations within Ames city limits.|
|**condition1**|*object*|train_cleaned.csv|Proximity to various conditions.|
|**bldgtype**|*object*|train_cleaned.csv|Type of dwelling.|
|**housestyle**|*object*|train_cleaned.csv|Style of dwelling.|
|**overallqual**|*int*|train_cleaned.csv|Rates the overall material and finish of the house.|
|**overallcond**|*int*|train_cleaned.csv|Rates the overall condition of the house.|
|**roofstyle**|*object*|train_cleaned.csv|Type of roof.|
|**exterior1st**|*object*|train_cleaned.csv|Exterior covering on house.|
|**exterior2nd**|*object*|train_cleaned.csv|Exterior covering on house. (if more than one material)|
|**masvnrtype**|*object*|train_cleaned.csv|Masonry veneer type.|
|**masvnrarea**|*float*|train_cleaned.csv|Masonry veneer area in square feet.|
|**extercond**|*object*|train_cleaned.csv|Evaluates the present condition of the material on the exterior.|
|**foundation**|*object*|train_cleaned.csv|Type of foundation.|
|**bsmtqual**|*int*|train_cleaned.csv|Evaluates the height of the basement.|
|**bsmtexposure**|*int*|train_cleaned.csv|Refers to walkout or garden level walls.|
|**bsmtfintype1**|*object*|train_cleaned.csv|Rating of basement finished area.|
|**totalbsmtsf**|*float*|train_cleaned.csv|Total square feet of basement area.|
|**heatingqc**|*int*|train_cleaned.csv|Heating quality and condition.|
|**1stflrsf**|*float*|train_cleaned.csv|First Floor square feet.|
|**grlivarea**|*object*|train_cleaned.csv|Above grade (ground) living area square feet.|
|**bsmtfullbath**|*int*|train_cleaned.csv|Basement full bathrooms.|
|**fullbath**|*int*|train_cleaned.csv|Full bathrooms above grade.|
|**halfbath**|*int*|train_cleaned.csv|Half baths above grade.|
|**bedroomabvgr**|*int*|train_cleaned.csv|Bedrooms above grade. (does NOT include basement bedrooms)|
|**totrmsabvgrd**|*int*|train_cleaned.csv|Total rooms above grade. (does not include bathrooms)|
|**fireplaces**|*int*|train_cleaned.csv|Number of fireplaces.|
|**garagetype**|*object*|train_cleaned.csv|Garage location.|
|**garagefinish**|*object*|train_cleaned.csv|Interior finish of the garage.|
|**garagearea**|*float*|train_cleaned.csv|Size of garage in square feet.|
|**saletype**|*object*|train_cleaned.csv|Type of sale.|
|**saleprice**|*float*|train_cleaned.csv|Condition of sale.|
|**houseage**|*int*|train_cleaned.csv|Age of the house when it was sold.|
|**renoage**|*int*|train_cleaned.csv|Number of years since the house was last remodeled.|
|**outdoorfeature**|*bool*|train_cleaned.csv|Whether house has outdoor features like a deck or porch.|

# Credits
Test.csv [Source](https://www.kaggle.com/c/dsi-us-6-project-2-regression-challenge/data)

Train.csv [Source](https://www.kaggle.com/c/dsi-us-6-project-2-regression-challenge/data)
