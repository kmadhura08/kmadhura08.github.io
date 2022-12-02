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
The original dataset consists of data from 2017 to October 2022. But, we decided to go with 2021 data and the 2022 data. The data that we decided to got with was very large in intself and hence, we downsampled the data to 50,000 observations to make the visualizations. The EDA and the code to get the final data can be found <a href="https://github.com/kmadhura08/kmadhura08.github.io/blob/main/python_notebooks/Final-Project-Data-Pre-processing.ipynb">here</a>

### Rides per bike-type VS Year

<vegachart schema-url="{{ site.baseurl }}/assets/json/jsonride_year.json" style="width: 100%"></vegachart>

Cook County has the highest amount of square feet, followed by Champaign and Sangamon, according to this interactive plot of square footage by counties in the state of Illinois. We are collecting data from the specified link. The visualization is 250 wide by 1000 high, and it shows the number of counties and their square footage on the x and y axes, respectively. The color scheme used is green since it is visually appealing and represents the amount of land each county has been used for. We applied data transformation by eliminating null values and adding up the square footage. Quantitative and nominal encoding types were used for this plot. Similar to what Himank did in his Assignment 9 quite a bit. Major changes include adding the command interactive and converting tooltip contents to plot. These changes provide us all the information we need to quickly and thoroughly analyze each bar in a bar chart.


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



