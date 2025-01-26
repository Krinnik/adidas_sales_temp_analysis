#
## __Adidas Product Sales vs. US Temperature Analysis__

## __Summary__

* This analysis __investigates__ the __Correlation__ between __Average US Regional Temperatures__ and __Adidas Product Sales__ across __five core regions__: 
    * __Northeast__
    * __Southeast__
    * __Midwest__
    * __South__
    * __West__
* This analysis also __utilizes Prophet__ to __forecast category sales__ across __each region__.

* __Key Findings__:
    * __Temperature significantly correlates__ with __sales__ in the __Southeast__ and __South__ regions.
    * The __Northeast__ shows __minimal correlation__ between __temperature__ and __sales__.
    * The __Midwest__ and __West__ exhibit moderate correlations.
    * __Prophet Findings__:
        * __Northeast__ and __South__: __Projected__ to deliver the __highest overall growth__.
        * __Southeast__: __Projected__ to deliver __moderate growth__.
        * __Midwest__: __Projected__ to __remain nearly flat__.
        * __West__: __Projected__ to experience a __decline in sales across the board__. 

* __Recommendations__:
    * __Implement targeted marketing campaigns__ during __periods of rising temperatures__ in __regions__ with __strong correlations__.
    * __Develop region-specific product launches__ and __collaborations__ to __capitalize on seasonal trends__.
#
## __Data Cleaning and Methodology__

* __Adidas Sales Data__: 
    * We used a __2020/2021 product sales dataset__: (https://www.kaggle.com/datasets/heemalichaudhari/adidas-sales-dataset)
* __Temperature Data__: 
    * __Monthly temperature data__ by __state from 1950-2022__: (https://www.kaggle.com/datasets/justinrwong/average-monthly-temperature-by-us-state).
* __Data Cleaning__: We addressed __missing data__ and __inconsistencies__ in __both datasets__ to __ensure accurate analysis__. Such as: 
    * The __initial Total Product Sales__ data being __miscalculated__
    * __Most States/Regions__ were __missing 2021 Data__
    * __Minor Temperature increments__ caused __"Lumpy Data"__ in graphs
* __Correlation Analysis__: We calculated __correlation coefficients__ to __assess__ the __relationship__ between __temperature__ and __sales__ in __each region__.
#
## __Foundational Adidas Sales Insights__

* __Street Footwear__ is the __largest__ overall __category__, followed by __Apparel__.
* The __West__ region contributes the __largest share__ of __total sales__, followed by the __Northeast__. The __South__ is the __smallest__ region overall.
* __Street Footwear__ is the __leading category__ across __each region__.
* __Athletic Footwear__ is the __smallest category__ across __each region__.
#
![category sales by region](<Resources/readme_screenshots/Screenshot 2025-01-26 115844.png>)
#
## __Regional Sales Trends__

* __Southeast__ & __Midwest__: 
    * Sales __increase__ in __June/July__.
* __South__: 
    * Sales __significantly ramp up__ in __September__.
* __Northeast__: 
    * Sales __grow__ in __November/December__.
* __Overall__: 
    * __March__ is the __slowest month__ for __total sales__.
* __Athletic Footwear__: 
    * __Peaks__ in __January__ (New Year's Resolution) and __August/September__ (Back to School).
* __Apparel__: 
    * __Peaks__ in __June/July__ (Summer) and __November__ (Holiday Gifting).
#
![comparison of sales by month and region](<Resources/readme_screenshots/Screenshot 2025-01-26 115935.png>)
#
## __Temperature by Region Insights__

* The __Midwest__ has the __biggest temperature differentials__ across months.
* The __South__ shows the __hottest temperatures overall__ during __summer__.
* The __Midwest__ shows the __coldest temperatures__ during __winter__.
#
![average temperature by region and month](<Resources/readme_screenshots/Screenshot 2025-01-26 120141.png>)
#
## __Regional Temperature Correlation with Sales__

* The __Southeast__ and __South__ regions have the __strongest correlation__ between __temperature and sales__.
* There is __almost no correlation__ between __temperature and sales__ in the __Northeast__.
* The __Midwest__ and __West__ exhibit __low to moderate correlations__, with the __West__ showing __nearly double__ the __correlation__ compared to the __Midwest__.
#
![regional temperature correlation with sales](<Resources/readme_screenshots/Screenshot 2025-01-26 124515.png>)
#
## __Category Sales Forecast by Region using Prophet Predictions__

* __Northeast__ region is __projected__ to deliver __highest overall growth__.

* __South__ region is __projected__ to deliver __significant growth__ as well. 

* __Southeast__ is __projected__ to deliver __moderate growth__

* __Midwest__ is __projected__ to be __nearly flat__. 

* __West__ is __projected__ to __decline across the board__.
#
![projected growth rates by category and region](<Resources/readme_screenshots/Screenshot 2025-01-26 120343.png>)
#
## __Conclusions by Region__

### __Midwest__

* __Forecast__: 
    * __Flat growth__ through __June 2023__, with a __slight decline__ in __Street Footwear sales__ (concerning, as it __contributes 40% of total sales__).
* __Analysis__: 
    * __Moderate correlation (0.06)__ between temperature and sales.
* __Recommendations__:
    * __Holistic promotion__ across __all categories__ during __April__ and __August__ (rising temperatures).
    * __Additional Street Footwear promotion__ in __April__ to __address expected sales loss__.
    * Consider __regional product launches aligned__ with the __region__ and __College football season__.
    * Leverage __September's still-hot temperatures__ and __Back to School timing__ for __Apparel__ and __Street Footwear__.

![midwest graph](<Resources/readme_screenshots/Screenshot 2025-01-26 122412.png>)
![midwest forecast](<Resources/readme_screenshots/Screenshot 2025-01-26 122623.png>)

### __Northeast__

* __Forecast__: 
    * __Moderate growth__ through __June 2023__, with __Street Footwear__ and __Apparel__ increasing their share of sales. __Athletic Footwear__ sales are __not expected to accelerate__ as quickly.
* __Analysis__: 
    * __Low correlation (0.004)__ between __temperature__ and __sales__.
* __Recommendations__:
    * __Holistic promotion__ across __all categories__ during __April__ and __August__ (rising temperatures).
    * Consider __regional product launches__ or __collaborations aligned__ with __these periods__.
    * Leverage __September's still-hot temperatures__ and __Back to School timing__ for __Apparel__ and __Street Footwear__.
    * Consider __regional product launches__ or __promotions aligned__ with __College football season__.

![northeast graph](<Resources/readme_screenshots/Screenshot 2025-01-26 122729.png>)
![northeast forecast](<Resources/readme_screenshots/Screenshot 2025-01-26 122419.png>)

### __South__

* __Forecast__: 
    * __Significant growth__, with the __highest__ coming __from Street Footwear__. __Apparel sales__ are __projected to slow__.
* __Analysis__: 
    * __Higher correlation (0.30)__ indicates __underperformance during May-August__.
* __Recommendations__:
    * __Holistic promotion__ across __all categories__ from __May through August__ (summer months).
    * __Additional emphasis__ on __Apparel__ to __reverse forecasted decline__:
    * Consider __regional product launches__ or __collaborations specific__ to __"Summer in the South."__
    * Consider __additional regional product launches__ associated with __College football season__.

![south graph](<Resources/readme_screenshots/Screenshot 2025-01-26 123410.png>)
![south forecast](<Resources/readme_screenshots/Screenshot 2025-01-26 123358.png>)

### __Southeast__

* __Forecast__: 
    * __Slight overall growth__, but leading categories __(Street Footwear and Apparel)__ are __projected to decline__.
* __Analysis__: 
    * __Highest overall correlation (0.40)__ between __sales__ and __temperatures__.
* __Recommendations__:
    * __Holistic promotion__ across __all categories__ to drive __incremental volume__ in __April__ and __August__, aligned with __rising temperatures__.
    * Consider __regional product LTO__ or __collab__ during __these periods__ specific to the region.
    * __Additional opportunity__ in __September__ for __Apparel__ based on __'still-hot' temperatures__ and __Back to School timing__ to __reverse forecast declines__.
    * Consider __regional product launch aligned__ with __College football season__.

![southeast graph](<Resources/readme_screenshots/Screenshot 2025-01-26 123446.png>)
![southeast forecast](<Resources/readme_screenshots/Screenshot 2025-01-26 123436.png>)

### __West__

* __Forecast__: 
    * __Overall__, the __West__ region is __projecting declines__ across __all categories__.
* __Analysis__: 
    * __Moderate overall correlation (0.09)__ between __sales__ and __temperatures__.
* __Recommendations__:
    * __Holistic promotion__ across __all categories__ to drive __incremental volume__ from __June__ through __August__.
    * Consider __regional product LTO__ or __collab aligned__ with the __region__.
    * __Additional opportunity__ in __September-October__ for __Apparel__ based on __'still-hot' temperatures__ and __Back to School timing__ to __reverse forecast declines__.
    * Consider __regional product launch aligned__ with __College football season__.

![west graph](<Resources/readme_screenshots/Screenshot 2025-01-26 123543.png>)
![west forecast](<Resources/readme_screenshots/Screenshot 2025-01-26 123536.png>)
#
## __Dependencies__:
    - pandas
    - Prophet
    - datetime
    - numpy
    - matplotlib.pyplot
    - %matplotlib inline
#
## __Data Sources__:

* __Adidas product / sales database__:  https://www.kaggle.com/datasets/heemalichaudhari/adidas-sales-dataset
    * __Product Sales Data from 2020-2021 ranging from state, retailer, product type, units sold, etc__.
* __Monthly temperature by state dataset__: https://www.kaggle.com/datasets/justinrwong/average-monthly-temperature-by-us-state
    * __Average Monthly Temperature__ by __State ranging from 1950-2022__.




