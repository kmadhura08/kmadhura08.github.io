---
name: Homework#10
tools: [Python, Altair, vega-lite, Jekyll]
image: assets/pngs/cars.png
description: This is a introductory assignment to altair, vegalite and python!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Homework#10
## By- Himank Dave and Madhura Kulkarni


<vegachart schema-url="{{ site.baseurl }}/assets/json/jsonsq_footage.json" style="width: 100%"></vegachart>
<vegachart schema-url="{{ site.baseurl }}/assets/json/jsonfloors.json" style="width: 100%"></vegachart>

{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/building_inventory.csv" text="The Data" %}
{% include elements/button.html link="https://github.com/kmadhura08/kmadhura08.github.io/blob/main/python_notebooks/Assignment_10.ipynb" text="The Analysis" %}



