## Learning Objectives


* Why Dash?
* What is Dash?
* Example
* Installing Dash
* Dash App Layout
* Getting Started
* Styling the app
* Creating and Viewing Visualizations
* Core Components




## Why Dash?


* Using the plotly python library by itself creates interactive plots as .html files.
* While users can still interact with these plots (zoom in, select, hover over), these plots can’t be connected to changing data sources. You would need to re-run the .py script and re- generate the .html file to see any updates.
* Having to re-run .py scripts is not really what we want while we’re thinking about dashboards. We want it to be updated automatically whenever the data changes.
* This is where we need something like Dash.



## What is Dash?


Dash is a user interface library/ Python framework for creating analytical web applications. Those who use Python for data analysis, data exploration, visualization, modelling, instrument control, and reporting will find immediate use for Dash.

It is built on top of Flask, Plotly.js, React and React Js. It enables you to build dashboards using pure Python. Dash is open source, and its apps run on the web browser. Every aesthetic element of the app is customizable: The sizing, the positioning, the colors, the fonts.

## Example

Here’s an example of a Dash app for fertility rate and life expectancy:






![image1.gif](https://dphi-live.s3.amazonaws.com/media_uploads/image1_18c9fb4b7aeb44d985b5fc595a68697f.gif)






### Dash App gallery

Explore the Dash App gallery here: 

https://dash-gallery.plotly.host/Portal/

## Installing Dash

Dash can be installed with a simple line of code:

`pip install dash`

## Dash App Layout

A Dash application is usually composed of 3 pillars:
1. Dash Components - Components like slider, checkbox, dropdown
in order to give your application an interactive capability
2. Plotly Graphs - Data Visualization plots that allow the user to visualize the data
3. The Callback - One of the most important elements. It connects Dash Components and Plotly Graphs in order to create an interactive capability.

The Dash Components and Plotly Graphs are inside the app layout and describes how the app will look like and the Callback describes the interactivity of the application and is outside app layout.

Dash provides HTML classes that enable us to generate HTML content with Python. To use these classes, we need to import dash_core_components and dash_html_components.

* We use the Div class from the dash_html_components to create an HTML Div. We then use the HTML components to generate HTML components such as H1, H2 etc. dash_html_components has all HTML tags.
* In order to create a graph on our layout, we use the Graph class from dash_core_components. Graph renders interactive data visualizations using plotly.js. The Graph class expects a figure object with the data to be plotted and the layout details.

## Getting Started

### For working with Dash Locally with a Text Editor

To kick us off we shall create a file called app.py using our favorite text editor (you can use Sublime Text, VSCode or any other text editor).

### For working with Dash in Jupyter Notebook or Colab 
__(Doesn’t work in Colab properly sometimes)__

If you don’t wish to run Dash locally on a text editor on your device but instead want to use a Jupyter Notebook environment, you can use JupyterDash (https://pypi.org/project/jupyter-dash/).

Note: JupyterDash often doesn’t work with Colab correctly. You can refer to this demo on Colab and see if it works for you:

https://colab.research.google.com/gist/xhlulu/73ffc0b920d72142ac1db5f1026616b0/jupyterdash-demo.ipynb

We’ll first import these packages.

```
import dash
import dash_core_components as dcc
import dash_html_components as html
```

## Styling the app/dashboard (dash_html_components)


Dash also allows you to do stylings such as changing the background color and text color. You can change the background by using the style attribute and passing an object with your specific color. Similarly, we can change the layout background using the plot_bgcolor attribute.

Customizing your dashboard is similar to using HTML. If you’re familiar with HTML, it will come handy here. If not, you can surely follow along and learn.

There are some apparent differences between HTML and Dash Syntax though. In HTML the style property is specified using a semicolon, but in Dash, a dictionary is supplied. The keys in the dictionary are camelCased e.g text-align is textAlign. Instead of using classes like in HTML, className is used in Dash.






![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_7d1b74045bb04987a09e13d2abf5c04e.png)








## Creating Visualizations (dash_core_components)









![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_df086decd5c640feb777bf2abe2baaa3.png)








## View the Visualization

In order to view our visualization, we need to run our web server
just like in Flask (a Python tool to build web applications). Remember Dash is built on top of Flask. We also set debug to true to ensure we don't have to keep refreshing the server every time we make some changes.


![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_1325f52dfee243c58db35ec9e3edd6f6.png)




## Running the Application Locally

Next, move to the terminal and start the server by typing the code below: 

`python app.py`

This will start a new web server at http://127.0.0.1:8050/. Head over there and see your newly created dashboard.




![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_74d2521a805246abb59c75d63f4a5264.png)





## Core Components

Next, let's look at some dash_core_components that you will encounter when using Dash.
* You can generate a drop down by calling Dropdown from
dash_core_components and passing the options as a list of dictionaries.
* Radio buttons can be generated using the RadioItems attribute.
* To generate checkboxes, you can call the Checklist attribute.
* To use input texts in your application, you will use the Input attribute.

That’s how your application will look like by using these components:




![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_263a38db7063404b9132f80a2d5f1186.png)






## Seeking Help

Stuck somewhere? Don’t know what a particular Dash component
does or want to know more about how to use it?

Since Dash components are declarative, calling the help command
on any of them will generate the help for that component.
`help(dcc.Input)`

## References

* https://www.datacamp.com/community/tutorials/learn-build-dash-python

## Slide Download Link
You can download the slides for this topic from [here](https://docs.google.com/presentation/d/14HD7TKebXcSSUP7KZnnVnFkltSFMZxVhdUV7RlKckJU/edit?usp=sharing).