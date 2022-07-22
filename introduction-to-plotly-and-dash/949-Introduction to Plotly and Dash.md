## Learning Objectives

* What is Plotly?
* Why Plotly?
* Disadvantages of Plotly
* How is it different from other DV libraries?
* Why it’s great for data scientists and engineers
* Why Dash?
* What is Dash?


## What is plotly?






![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_e673b14844db4d7d901a79b0d8572912.png)





* The name ‘Plotly’ can cause confusion because it is both a
company and an open-source library
* Plotly the company focuses on data visualization for business intelligence: such as reporting, dashboards and BI solutions. They make it easy to create, deploy, and share interactive web apps, graphs, and visualizations in any programming language.
* The company released an open-source library called Plotly which is a general data visualization library focused on interactive visualizations. This will be the focus of our course.
* Plotly is a Javascript graphing library. But don’t worry, you
don’t need to know Javascript for using it.
* It is compatible with a number of languages/ tools: R, Python, MATLAB, Perl, Julia, Arduino.
* The most popular version is the Python library.
* Plotly has a Python wrapper i.e we will write code in Python and it will produce Javascript code.

## Why Plotly?

* It is fast and easy to implement simple plots.
* Can also be used by people with no technical background for creating interactive plots by uploading the data and using plotly GUI.
* plotly.express allows to create plots with less code and effort.
* It lets you create interactive visualizations.
* It provides compatibility with number of different languages/ tools.
* Interactive plots can easily be shared online with multiple people.
* It allows to embed interactive plots in projects or websites using iframes or html.
* It is extremely customizable.

## Disadvantages of Plotly

* The plots made using plotly community version are always
public and can be viewed by anyone.
* For plotly community version, there is an upper limit on the API calls per day.
* There are also limited number of color Palettes available in community version which acts as an upper bound on the coloring options.

## How is it different from other DV libraries?

There are definitely other tools out there that can help you plot your data, such as Matplotlib, Seaborn, Bokeh, and even D3 if you want to build a visualization dashboard.

However, developing fancy web apps comes with the long time to build and a steep learning curve. This is the sweet spot that Plotly has over other tools, which makes visualizing data at any scale much easier for data scientists.

If you or your clients are looking to have some interactions with your graphs, Plotly might be a good shot to try. Built on top of Plotly JavaScript library (plotly.js), plotly.py enables users to create beautiful interactive web-based visualizations that can be displayed in Jupyter notebooks, saved to standalone HTML files, or served as part of pure Python-built web applications using Dash (we’ll learn about Dash soon).

While Seaborn and Matplotlib graphics are static, Plotly charts allow you to hover over values and zoom in/out your graphs, like identifying outliers among a large number of data points or detecting anomalies in time series plots.

## Why it’s great for data scientists and engineers

Most of data scientists and engineers write in Python. Their roles oftentimes require them to be able to aggregate small and big datasets fluently, to manipulate any kinds of data efficiently, and to work with libraries like Pandas. Plotly allows us to build charts for the web right from Pandas dataframe.

Also, building interactive charts with Javascript can be a steep learning curve for non front-end engineers. Plotly allows for interactive plotting from a commonly used scripting language like Python/R. It’s built on top of d3.js (a visualization library) and stack.gl (helps in assembling 3D scenes).

## Why Dash?
* Using the plotly python library by itself creates interactive plots as .html files.
* While users can still interact with these plots (zoom in, select, hover over), these plots can’t be connected to changing data sources. You would need to re-run the .py script and re- generate the .html file to see any updates.
* Having to re-run .py scripts is not really what we want while we’re thinking about dashboards. We want it to be updated automatically whenever the data changes.
* This is where we need something like Dash.

## What is Dash?

Often users want plots to be able to interact with each other, interact with components, or have plot updates in real time. To accomplish this level of tasks, we need a dashboard! (which is a step beyond what normal plotly can provide for us).

Dash is an open source library from the Plotly company that allows you to create a full dashboard with multiple components, interactivity and multiple plots.

To fully understand Dash, we should first get comfortable with Plotly!

### Slide Download Link

You can download the slides for this topic from [here](https://docs.google.com/presentation/d/18dOeT7FOzOadhTZLqNW0RdxAv1dejSfuX1GTkNGxjuA/edit?usp=sharing).

### References

* https://www.analyticsvidhya.com/blog/2017/01/beginners-guide-to-create-beautiful-interactive-data-visualizations-using-plotly-in-r-and-python/