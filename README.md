# Interactive-Data-Visualisation-with-Bokeh-for-Astronomers
Basic Bokeh tutorial presented at an ESO Chile Python Coffee. 

The focus is on the applications to the analysis of astronomical data.

Title: 
Interactive Data Visualisation with Bokeh: A Beginner’s Tutorial
 
Abstract:
Clear and interactive visualisations are a useful tool for data analysis, particularly for large and cross-correlated databases. Bokeh is a Python library that enables the creation of customised, interactive plots for the web (and for your personal notebooks), without requiring JavaScript. This tutorial introduces the fundamentals of Bokeh, focusing on how to build basic, interactive plots. Participants will learn how to work with Bokeh’s core components, such as figures, glyphs, layouts, and data sources, and will gain hands-on experience in creating dynamic dashboards. Participants are invited to discuss particular uses for their respective science cases.

![](Basic_Interactive_Plot.png)

### Requisites

Install Bokeh by running:

```
pip install bokeh
```

or

```
conda install bokeh
```

in a terminal. All the required packages should be installed automatically.

The step by step tutorial for begginers is in the following jupyter notebook: [Basics_of_Bokeh_for_Astronomy.ipynb](Basics_of_Bokeh_for_Astronomy.ipynb). 

The first part explains how to read the data from a pdf file using the python library [camelot](https://camelot-py.readthedocs.io/en/master/). However, to run the tutorial the user just needs to download the [data.csv](data.csv) file and skip the "! Read data from pdf and convert to csv table" section.

### Questions asked during the tutorial

##### Q1. Is it posible to use latex text to set the names of the axis in plots?
It is. The user just needs to use any of the following delimiters to capsule the string: $$...$$, \[...\], and \(...\). For example: r"$$\sin(x)$$". This feature is now available in the tutorial.

For more information visit the [Bokeh Mathematical Notation Documentation](https://docs.bokeh.org/en/latest/docs/user_guide/styling/mathtext.html#ug-styling-mathtext)

This question has also been answered in the [Bokeh Community Forum](https://discourse.bokeh.org/t/legend-with-latex-or-imageurl/9160)

##### Q2. Is it posible to link a different plot to the points to display it when hovering?
It is. You can link a locally stored image to each point in a dataset, pass the Pathname to Bokeh and make it display the image when hovering over the plot. Find an example in the following jupiter notebook: More_Advances_Examples_of_Bokeh_for_Astronomy.ipynb

The user will need to provide their own data for this example. An useful discussed implementations is linking spectra to points in a temporal series. 

### License and citation
Bokeh is BSD licensed, so you are free to use it however you like, as long as you copy the BSD statement if you redistribute the Bokeh source code (see [LICENSE.txt](https://github.com/bokeh/bokeh/blob/1.1.0/LICENSE.txt) for full details).

However, if you find Bokeh useful in your work, developers appreciate a citation.

To cite Bokeh in publications, use:
```
Bokeh Development Team (2018). Bokeh: Python library for interactive visualization
URL http://www.bokeh.pydata.org.
```
A BibTeX entry for LaTeX users is:

```
@Manual{,
title = {Bokeh: Python library for interactive visualization},
author = {{Bokeh Development Team}},
year = {2018},
url = {https://bokeh.pydata.org/en/latest/},
}
```
