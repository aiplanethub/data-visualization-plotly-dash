## Learning Objectives


* Installing Plotly
* Creating Plotly Figures
* Typical steps for creating interactive plots
* The Plotly Figure
* Getting started with Plotly and Building a Pie Chart
* Creating and Formatting Bar Chart


## Installing Plotly


plotly can be installed using pip:
`pip install plotly==4.14.3`

or conda:

`conda install -c plotly plotly=4.14.3`

PS: plotly comes pre-installed in Google Colab.


## Creating Plotly Figures


Plotly graphs can be created:

1. With plotly.express for simple, quick plots (imported as px)
   * Specify a DataFrame and its columns as arguments.
   * Quick and nice but less customization
2. With plotly.graph_objects (imported as go) for more
customization
   * go.X methods like go.Bar() and go.Scatter() allow many more customization options
   * Requires more code
3. With plotly.figure_factory for specific, advanced figures.





## Typical steps for creating interactive plots


1. Get the data to be used for creating visualizations and preprocess it to convert it into the desired format.
2. Call the Plotly API in the language/ tool of your choice.
3. Create the plot by specifying objectives like the data to be represented at each axis of the plot, the most appropriate plot type (like histogram, box plots, 3D surfaces), the color of data points, lines in the plot and other features.

Here's a generalized format for basic plotting in Python:

`plotly.plotly( [plotly.graph_objs .type(x ,y ,mode , marker = dict(color ,size ))]`

Where:

* x = values for x-axis
* y = values for y-axis
* type = to specify the plot that you want to create like "histogram", "surface", "box", etc.
* mode = format in which you want data to be represented in the plot. Possible values are "markers", "lines, "points".
* color = values of the same length as x, y, and z representing the color of data points or lines in the plot.
* size = values of the same length as x, y, and z representing the size of data points or lines in the plot.



## The Plotly Figure



A Plotly figure has three main components:

* Layout - a dictionary of attributes that control the look and
style of the figure.
  * There is one layout element per figure.
* data - a list of dictionaries that sets up the type of graph and the data to display.
  * data + type = a trace. There are over 40 types!
  * Can have multiple traces per plot.
* frames - For animated plots


## Getting started with Plotly and Building a Pie Chart

The video below will give a walkthrough of the following topics:

* Plotly Express vs. Plotly Graph Objects
* Navigating Plotly's documentation to create your graphs
* Building a Pie Chart and customizing it
* Getting support when you are stuck
* How to share your graphs with others

It will also be utilizing some links. You can open the document below for those:

https://drive.google.com/file/d/1KW975FyaM7l-91sxmE3OX3egi_UMh2ot/view

You can directly use the dataset with the link:

https://raw.githubusercontent.com/dphi-official/Datasets/master/bird-window-collision-death.csv











<iframe width="560" height="315" src="https://www.youtube.com/embed/_b2KXL0wHQg?start=253" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>












### Notebook Link - Pie Chart

All the operations performed in the video can be found in this notebook:

https://dphi.tech/notebooks/948/gunnika/getting-started-with-plotly-and-building-a-pie-chart

We strongly suggest creating a new notebook/python file of your own and working along the video. You can refer to the notebook whenever you are stuck!

## Bar Chart

The video below will give a walkthrough of building a bar
chart.

You can directly use the dataset with the link:

https://raw.githubusercontent.com/dphi-official/Datasets/master/Caste.csv








<iframe width="560" height="315" src="https://www.youtube.com/embed/N1GwQNatOwo?start=120" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>







### Notebook Link - Bar Chart
All the operations performed in the video can be found in this notebook:

https://dphi.tech/notebooks/949/gunnika/creating-and-customizing-bar-charts-in-plotly

We strongly suggest creating a new notebook/python file of your own and working along the video. You can refer to the notebook whenever you are stuck!

### Slide Download Link
You can download the slides for this topic from [here](https://docs.google.com/presentation/d/1mZQ82PeoLN6w0kL9HhUBA4fQ5Lkrx2B5FOtGJ5hPRFU/edit?usp=sharing).

### References
* https://www.analyticsvidhya.com/blog/2017/01/beginners-guide-to-create-beautiful-interactive-data-visualizations-using-plotly-in-r-and-python/