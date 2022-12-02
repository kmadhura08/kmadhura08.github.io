---
name: Final_Project
tools: [Python, Altair, vega-lite, Jekyll]
description: This is an introductory assignment to altair, vegalite and python!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# How successful is Lyft at BayWheels?
<b>Team Members</b> - Himank Dave (hjdvae2) and Madhura Kulkarni (msk10)

Bay Wheels is a regional public bicycle sharing system in the San Francisco Bay Area of California. Lyft Bikes and Scooters, LLC ("Bikeshare") operates the Bay Wheels bicycle sharing service. 
The <a href="https://www.lyft.com/bikes/bay-wheels/system-data">original data</a>
consists of data from 2017 to October 2022. But, we decided to go with 2021 and 2022 data. This was very large in in itself and hence, we downsampled the data to 50,000 observations to make the visualizations. Data includes rider's information regarding the type of the bike and details about the source and destination of the station. The EDA and the code to get the final data can be found
<a href="https://github.com/kmadhura08/kmadhura08.github.io/blob/main/python_notebooks/Final-Project-Data-Pre-processing.ipynb">here</a>

### Rides per bike-type VS Year

<vegachart schema-url="{{ site.baseurl }}/assets/json/jsonride_year.json" style="width: 100%"></vegachart>

We were interested to find out the most-used bike-type. In the above visualization, we can see the distribution of number of rides over different bike-types in the year 2021 and 2022. Surprisingly, the number of rides taken for the docked bike is extremely less as compared to the other two-bike types.


Moving forward, we wanted to know the subscription pattern of the riders. From the above nested pie chart, we can conclude that number of casual riders and member riders are fairly the same in 2021 as well as 2022. One important thing to note down here is that our data has records till October 2022 and clearly the use of the Bikeshare service has increased than the past year.


### Contextual Visualizations
<vegachart schema-url="{{ site.baseurl }}/assets/json/nested.json" style="width: 100%"></vegachart>

This interactive graphic shows the number of floors for each usage category in the state of Illinois. Based on a quick glance, it is clear that storage has a high percentage of occupied floors.
Data is being gathered from the designated link. The Number of Floors per Usage Category is displayed on the x and y axes of the 800 wide by 350 high visualization, respectively. Nominal and quantitative encoding types were used for this plot as well as it serves the best when building a bar chart. The color scheme chosen is blue since it looks well and reflects how much land has been exploited by each category. By removing null values and adding the floors, we transformed the data. Quite a bit like what Himank accomplished in his Assignment 9. The command interactive has been added, and the contents of tooltips have been converted to plot. All the information we require to swiftly and in-depthly study each bar in a bar chart is provided by these changes.

<div class="left">
{% include elements/button.html link="https://media.githubusercontent.com/media/kmadhura08/kmadhura08.github.io/main/python_notebooks/small_data.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/kmadhura08/kmadhura08.github.io/blob/main/python_notebooks/Final_Project_Part_3.ipynb" text="The Analysis" %}
</div>



