---
name: Final_Project
tools: [Python, Altair, vega-lite, Jekyll]
description: This is the final project for the course IS 445-Data Visualization
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
<img src="{{ site.baseurl }}/assets/pngs/nested_Pie.png" width="400" height="400"/>

Moving forward, we wanted to know the subscription pattern of the riders. From the above nested pie chart, we can conclude that number of casual riders and member riders are fairly the same in 2021 as well as 2022. One important thing to note down here is that our data has records till October 2022 and clearly the use of the Bikeshare service has increased than the past year.
### Contextual Visualizations

For contextual visualizations, we decided to go with one of the popular bike-sharing services in United States which is the <a href="https://ride.citibikenyc.com/system-data">Citi-bike</a>
for NYC. For our analysis, due to memory constraints, we used the data for the year 2021 only. The below two visualizations were built in Tableau.
<div class="left">
    <img src="{{ site.baseurl }}/assets/pngs/bar_chart.png" width="500" height="600">
</div>
<div class="right">
<img src="{{ site.baseurl }}/assets/pngs/pie_chart.png" width="500" height="600">
</div>
<br><br><br>
From the above visualizations, we can infer that number of riders riding the docked-bike is significantly high and most of the riders using the citi-bike service are subscribed to their service. The main conclusion to conclude from all the above visualizations is that Baywheels team definitely need to consider their low docked-bike riders and how they can increase their subscribers for overall popularity and profit.


<div class="left">
{% include elements/button.html link="https://media.githubusercontent.com/media/kmadhura08/kmadhura08.github.io/main/python_notebooks/small_data.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/kmadhura08/kmadhura08.github.io/blob/main/python_notebooks/Final_Project_Part_3.ipynb" text="The Analysis" %}
</div>



