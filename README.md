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

After checking ensuring the source data was ready to be read, the .csv files are imported into a Jupyter Notebook, merged together and analysed. Here are some of the key findings. 

### Results 1: Ride Counts by Area

Not surprising here, but what is interesting is the huge spread in urban areas. 
The outlier in the urban areas is West Angela, with 39 rides.

![ride count boxplot](https://github.com/carlosjennings1991/PyBer_Analysis/blob/main/Resources/Fig2.png)

The box & whisker chart above does a good job of showing the central tendencies, but for a quick snapshot, here is the same data in pie-chart form. 

![ride count piechart](https://github.com/carlosjennings1991/PyBer_Analysis/blob/main/Resources/Fig6.png)

---

### Results 2: Driver Counts by Area

Overall, not too surprising. 

![driver count boxplot](https://github.com/carlosjennings1991/PyBer_Analysis/blob/main/Resources/Fig4.png)
