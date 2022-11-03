---
name: Take 2 - vega-lite, many ways
tools: [Python, HTML, vega-lite, Jekyll]
image: assets/pngs/cars.png
description: Multiple ways to use vega-lite in our Jekyll page.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# General ways to include vega-lite plots

Order of operations:

1. generate a JSON specification (from somewhere -- vega-editor, 
Altair, etc)
1. save the JSON specification into `assets/json`


## 1. Including vega-lite plots directly from the editor





<vegachart schema-url="{{ site.baseurl }}/assets/json/fromvegaeditor.json" style="width: 100%"></vegachart>


<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/vega/vega/blob/main/docs/data/cars.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="The Analysis" %}
</div>

