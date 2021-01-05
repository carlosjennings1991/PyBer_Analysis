# PyBer Analysis

This analysis reviews the data for a ride-sharing app named "PyBer". There is a lot of information to digest, but the purpose is straightforward. Namely, we want to see the relationships between area type, driver count, and revenue. Throughout this study we will look to see if there's any surprising trends, outliers and relevant datapoints to inform the allocation of resources for the app. Here's what we'll review:
<br />

* **Total Revenue per Area Type (Urban, Suburban, Rural)**
* **Driver Count (per area)**
* **Avg Fare per Ride (per area)**
* **Avg Fare per Driver (per area)**


### Source Data can be found [here](https://github.com/carlosjennings1991/PyBer_Analysis/blob/main/Resources/PyBer_ride_data.csv)
### Analysis can be found [here](https://github.com/carlosjennings1991/PyBer_Analysis/blob/main/PyBer_Challenge_starter_code.ipynb)
---

## Results

After ensuring the source data was ready to be read, the .csv files are imported into a Jupyter Notebook, merged together and analized. Here are some of the key findings. 

### Results 1: Ride Counts by Area

Not surprising here, rural areas are lower, urban is higher and suburban areas inbetween. 
The outlier in the urban areas is West Angela, with 39 rides.

![ride count boxplot](https://github.com/carlosjennings1991/PyBer_Analysis/blob/main/Resources/Fig2.png)

The box & whisker chart above does a good job of showing the central tendencies, but for a quick snapshot, here is the same data in pie-chart form. 

![ride count piechart](https://github.com/carlosjennings1991/PyBer_Analysis/blob/main/Resources/Fig6.png)

---

### Results 2: Driver Counts by Area

While these general trend of this result is to be expected, what is interesting is the huge spread within urban areas. The interquartile range within urban areas could fit the entirety of the suburban box & whisker diagram. 

![driver count boxplot](https://github.com/carlosjennings1991/PyBer_Analysis/blob/main/Resources/Fig4.png)

Here's the same data as above but in pie-chart format. 

![driver count piechart](https://github.com/carlosjennings1991/PyBer_Analysis/blob/main/Resources/Fig7.png)

---

### Results 3: Ride fares by Area

This is a bit surprising. While only 2.6% of drivers are in rural area, they contribute 6.8% of the revenue. Another surprising find from this data is that high variability within rural fares. For example, fares within the first quartiles of the rural data is lower than lower-bound outliers within the suburban data. While one could expect the rural data to be higher (due to longer trips), finding comparatively low rural fares is surprising. 

![revenue boxplot](https://github.com/carlosjennings1991/PyBer_Analysis/blob/main/Resources/Fig3.png)

Here's the same data in pie-chart form. 

![revenue_piechart](https://github.com/carlosjennings1991/PyBer_Analysis/blob/main/Resources/Fig5.png)

---

### Results 4: Revenue Charted by Month

Here we see a chart of revenue, by area, for the first third of 2019. 

![revenue line chart](https://github.com/carlosjennings1991/PyBer_Analysis/blob/main/Analysis/PyBer_fare_summary.png)

Overall, this is to be expected in absolute terms. Of course, urban revenue will be the highest subtotal. What is a bit surprising is the overperformance of rural and suburban areas. While urban highers see a very high volume of rides writ large, they are much shorter in duration. 

---
## Summary

While the below chart is dense and requires a moment or two to digest, it's vastly informative. 

![composite scatterplot](https://github.com/carlosjennings1991/PyBer_Analysis/blob/main/Resources/Fig9.png)

**Suburban areas have the best of both worlds, and are the only group to have a positive correlation between ride number and fare price i.e places with more rides also have higher fares. So, it would make sense to expand coverage in similar suburban areas.** 

Some of the urban fares are very low. So depending on the break-even cost, certain cities might not be worth the trouble. 

The revenue per driver is quite low in urban areas. While this could be a reflection of part-time drivers, it could also reflect an overabundance of drivers who ultimately drive down the average revenue. Now, if they still bring revenue to the company, it isn't a problem. However, it could generate discontentment within the driver community. There could be some sort of threshold that keeps drivers on or a way to discourage excess drivers in areas that are already well serviced. 
