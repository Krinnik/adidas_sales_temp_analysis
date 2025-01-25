## Adidas Product Sales vs. US Temperature Analysis

## Summary

This analysis __investigates__ the __correlation__ between __average US regional temperatures__ and __Adidas product sales__ across __five core regions__: __Northeast, Southeast, Midwest, South,__ and __West__.

* __Key Findings__:
    * __Temperature significantly correlates__ with __sales__ in the __Southeast__ and __South__ regions.
    * The __Northeast__ shows __minimal correlation__ between __temperature__ and __sales__.
    * The __Midwest__ and __West__ exhibit moderate correlations.
* __Recommendations__:
    * __Implement targeted marketing campaigns__ during __periods of rising temperatures__ in __regions__ with __strong correlations__.
    * __Develop region-specific product launches__ and __collaborations__ to __capitalize on seasonal trends__.

## Data Cleaning and Methodology

* __Adidas Sales Data__: We used a __2020/2021 product sales dataset__: (https://www.kaggle.com/datasets/heemalichaudhari/adidas-sales-dataset)
* __Temperature Data__: __Monthly temperature data__ by __state from 1950-2022__: (https://www.kaggle.com/datasets/justinrwong/average-monthly-temperature-by-us-state).
* __Data Cleaning__: We addressed __missing data__ and __inconsistencies__ in __both datasets__ to __ensure accurate analysis__. Such as: 
    * The __initial Total Product Sales__ data being __miscalculated__
    * __Most States/Regions__ were __missing 2021 Data__
    * __Minor Temperature increments__ caused __"Lumpy Data"__ in graphs
* __Correlation Analysis__: We calculated __correlation coefficients__ to __assess__ the __relationship__ between __temperature__ and __sales__ in __each region__.

## Foundational Adidas Sales Insights

* Street Footwear is the largest overall category, followed by Apparel.
* The West region contributes the largest share of total sales, followed by the Northeast. The South is the smallest region overall.
* Street Footwear is the leading category across each region.
* Athletic Footwear is the smallest category across each region.

## Regional Sales Trends

* Southeast & Midwest: Sales share increases in June/July.
* South: Sales significantly ramp up in September.
* Northeast: Sales grow in November/December.
* Overall: March is the slowest month for total sales.
* Athletic Footwear: Peaks in January (New Year's Resolution) and August/September (Back to School).
* Apparel: Peaks in June/July (Summer) and November (Holiday Gifting).

## Temperature by Region Insights

* The Midwest has the biggest temperature differentials across months.
* The South shows the hottest temperatures overall during summer.
* The Midwest shows the coldest temperatures during winter.

## Regional Temperature Correlation with Sales

* The Southeast and South regions have the strongest correlation between temperature and sales.
* There is almost no correlation between temperature and sales in the Northeast.
* The Midwest and West exhibit low to moderate correlations, with the West showing a nearly double correlation compared to the Midwest.

## Opportunities by Region

### Midwest

* Forecast: Flat growth through June 2023, with a slight decline in Street Footwear sales (concerning, as it contributes 40% of total sales).
* Analysis: Moderate correlation (0.06) between temperature and sales.
* Opportunities:
    * Holistic promotion across all categories during April and August (rising temperatures).
    * Additional Street Footwear promotion in April to address expected sales loss.
    * Consider regional product launches aligned with the region and College football season.
    * Leverage September's still-hot temperatures and Back to School timing for Apparel and Street Footwear.

### Northeast

* Forecast: Moderate growth through June 2023, with Street Footwear and Apparel increasing their share of sales. Athletic Footwear sales are not expected to accelerate as quickly.
* Analysis: Low correlation between temperature and sales.
* Opportunities:
    * Holistic promotion across all categories during April and August (rising temperatures).
    * Consider regional product launches or collaborations aligned with these periods.
    * Leverage September's still-hot temperatures and Back to School timing for Apparel and Street Footwear.
    * Consider regional product launches or promotions aligned with College football season.

### South

* Forecast: Significant growth, with the highest coming from Street Footwear. Apparel sales are projected to slow.
* Analysis: Higher correlation (0.30) indicates underperformance during May-August.
* Recommendations:
    * Holistic promotion across all three categories from May through August (summer months).
    * Additional emphasis on Apparel to reverse forecasted decline:
    * Consider regional product launches or collaborations specific to "Summer in the South."
    * Consider additional regional product launches associated with College football season.

### Southeast

* Forecast: Slight overall growth, but leading categories (Street Footwear and Apparel) are projected to decline.
* Analysis: Highest overall correlation (0.40) between sales and temperatures.
* Recommendations:
    * Holistic promotion across all 3 categories to drive incremental volume in April & August, aligned with rising temperatures.
    * Consider regional product LTO or collab during these periods, possibly specific to the region.
    * Additional opportunity in September for Apparel based on 'still-hot' temperatures and Back to School timing to reverse forecast declines.
    * Consider regional product launch aligned with College football season.

### West

* Forecast: Overall, the West region is projecting declines across all 3 categories.
* Analysis: Moderate overall correlation (0.09) between Sales & Temperatures.
* Recommendations:
    * Holistic promotion across all three categories to drive incremental volume from June through August.
    * Consider regional product LTO or collab aligned with the region.
    * Additional opportunity in September-October for Apparel based on 'still-hot' temperatures and Back to School timing to reverse forecast declines.
    * Consider regional product launch aligned with College football season.

## Data Sources:

* Adidas product / sales database:  https://www.kaggle.com/datasets/heemalichaudhari/adidas-sales-dataset
    * Product Sales Data from 2020-2021 ranging from state, retailer, product type, units sold, etc.
* Monthly temperature by state dataset: https://www.kaggle.com/datasets/justinrwong/average-monthly-temperature-by-us-state
    * Average Monthly Temperature by State Data ranging from 1950-2022.




