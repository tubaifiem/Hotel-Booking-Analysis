# Hotel Booking Data Analysis
## Abstract
In this paper, the analysis of data using Python Programming Language is studied. The very basic processes of data analysis like cleaning, transforming, modeling of data is briefly explained in this paper and focus more on exploratory data analysis of an already existing dataset and finding the insights. Some graphical analysis of the data from the dataset will be shown using different libraries and functions of Python. Here, a dataset named “Hotel Booking Analysis” is used to analyze and extract various information in both numerical and pictorial form.
## Introduction
Data are those raw facts and figures with no proper information hence need to be processed to get the desired information. While information is those results that we get after processing the raw data in different levels or extracted conclusions from a given dataset through a process called data analysis.

Data Analysis is simply the analysis of various data means cleaning the data, transforming it into an understandable form, and then modeling data to extract some useful information for business use or organizational use. It is mainly used in taking business decisions. Many libraries are available for doing the analysis. For example, NumPy, Pandas, Seaborn, Matplotlib, pyplot, etc.

**NumPy**: NumPy is a library written in Pythand on, used for numerical analysis in Python. It stores the data in the form of nd-arrays (n-dimensional arrays).

**Pandas**: Pandas is mainly used for converting data into tabular form and hence, make the data more structured and easy to read.

**Matplotlib**: Matplotlib is a data visualization and graphical plotting package for Python and its numerical extension NumPy that runs on all platforms.

**Seaborn**: Seaborn is a Python data visualization package based on matplotlib that is tightly connected with pandas data structures. The core component of Seaborn is visualization, which aids in data exploration and comprehension.

**Pyplot**: matplotlib.pyplot is a collection of command style functions that make Matplotlib work like MATLAB. Each Pyplot function makes some change to a figure.

Data visualization will help the data analysis to ma it more understandable and interactive by plotting or displaying the data in pictorial form. Pandas, a Python open-source package that deals with three different data structures:  series, data frames,and panels, solves the need of analyzing and visualization of data.

Data analysis using Python makes tasks easier since Python Programming language has many advantages over any other programming language. It has prominent features like being a high-level programming language (the codes are in human-readable form) it is easy to understand and use by any programmer or user. Many libraries and functions for statistical, and numerical analysis are available in Python. Moreover, the source code is freely available to anyone (free and open source).

This paper includes all the basic terms and functions which are much needed by a beginner to know what data analysis is. The paper is divided broadly into 4 sections. In section II, the main steps in data analysis will be discussed. In section III, data analysis using python will be studied with all the basic needs of python in doing data analysis and data visualization will aid the analysis by representing them in picture format. In section IV, the conclusion of the paper is given.

## Data Analysis

**1. Data requirements**

Data is the most important unit in any study. Data must be provided as inputs to the analysis based on the analysis’ requirements. The term “experimental unit” refers to the type of organization that would be used to gather data (e.g., a person or population of people). It is possible to identify and obtain specific population variables (such as height, weight, age, and salary). It doesn’t matter whether the data is numerical or categorical.

**2. Data Collecting:**

The collecting of data is simply known as Data Collecting. Data is gathered from a variety of sources, including relational databases, cloud databases, and other sources, depending on the study’ needs. Field sensors, such as traffic cameras, satellites, monitoring systems, and so on, can also be used as data sources.

**3. Data processing**

Data that are collected must be processed or organized for analysis. For instance, these may involve arranging data into rows and columns in a table format (known as structured data) for further analysis, often through the use of spreadsheet or statistical software like SQL.

**4. Data cleaning:**

The method of cleaning data after it has been processed and organized is known as data cleaning. It scans for data inconsistencies, duplicates, and errors, and then removes them. The data cleaning process includes tasks such as record matching, identifying data inaccuracy, data sort, outlier data identification, textual data spell checker, and data quality maintenance. As a consequence, it keeps us from having unexpected outcomes and assists us in delivering high-quality data, which is essential for a successful outcome.

**5. Exploratory data analysis:**
Once the datasets are cleaned and free of error, it can then be analyzed. A variety of techniques can be applied such as exploratory data analysis- understanding the messages contained within the obtained data and descriptive statistics- finding average, median, etc. Data visualization is also a technique used, in which the data is represented in a graphical format in order to obtain additional insights, regarding the information within the data.

**6. Modeling and algorithms:**

Mathematical formulas or models (known as algorithms), may be applied to the data in order to identify relationships among the variables; for example, using correlation or causation.

**7. Data product**

A data product is a computer application that takes data inputs and generates outputs, feeding them back into the environment. It may be based on a model or algorithm.

### Data Analysis using Python

In this section, data analysis using python will be studied. The most basic things like why using python for data analysis will be understood. Moreover, how anyone can start using python will be shown. The important libraries, the platforms, the dataset to carry out the analysis will be introduced. Usage of various python functions for numerical analysis are given along with various methods of plotting graphs or charts are discussed.

**Why using Python?**

Python is a high-level, interpreted, multi-purpose programming language. Many programming paradigms like procedural programming language and object-oriented programming are supported in python. It can be used for many applications, that includes statistical computing with various packages and functions. Moreover, it is easy to learn. It can be picked up by anyone including those who has less programming skills.

Some features of Python are as listed below:

* Open source and free
* Interpreted language
* Dynamic typesetting
* Portable
* Numerous IDE
* Packages used:
* Numpy
* Pandas
* Seaborn
* Matplotlib
* Platform used:
* Colab Notebook
* Dataset used:
* Hotel Booking Analysis

### Working with dataset
**Importing libraries:**

Libraries that would be used in the process of analysis are to be imported first. Here are the codes to import the libraries. import pandas as pd
import numpy as np
import matplotlib.pyplot as plt import seaborn as sns

**Importing dataset**

Here, the dataset (Hotel Booking Analysis) is imported in the Colab notebook.
data = pd.read_csv('/content/drive/MyDrive/Hotel Bookings.csv')

**Cleaning Data**

Removing unwanted data or null values are done in the process of data cleaning. So, first we need to check the dataset whether it contains any null value or empty cells. isnull() returns true in the entry where there is no value or NA value. And sum() is used together with isnull() to find the total number of null values in every column.

According to our needs for the analysis, we can extract some particular rows or records from the dataset. Here is an example to extract the top most and last rows from the dataset. Head() is used to extract the top-most data in the dataset. 5 is the default value of the head(). Here, the top 5 rows from the dataset are taken.

**Exploratory Data Analysis**

In statistics, exploratory data analysis is an approach of analyzing data sets to summarize their main characteristics, often using statistical graphics and other data visualization methods. A statistical model can be used or not, but primarily EDA is for seeing what the data can tell us beyond the formal modeling or hypothesis testing task. Exploratory data analysis was promoted by John Tukey to encourage statisticians to explore the data, and possibly formulate hypotheses that could lead to new data collection and experiments.

* Data types: Datatype refers to the type of data- int, object, float are the basic data types in python. Printing the types of data of all the columns in the dataset using dtypes-mydata.dtypes.


### **Graphical EDA**

Fundamentally, graphical exploratory data analysis is the graphical equivalent to conventional non-graphical exploratory data analysis. EDA that examines data sets in order to summarize their statistical characteristics by focusing on the same four main features, such as measures of central tendency, measures of spread, distribution form, and the presence of
outliers. We also divided GEDA into three categories: Univariate GEDA, Bivariate GEDA, and Multivariate GEDA. We’ll go through these important varieties in more detail in the following paragraphs and aspects of GEDA.

First, a subset of the dataframe is taken to analyses or visualize using it.


#### Univariate GEDA

**1. Bar Plot:** Matplotlib - Bar Plot. A bar chart or bar graph is a chart or graph that presents categorical data with rectangular bars with heights or lengths proportional to the values that they represent. The bars can be plotted vertically or horizontally. Bar Plot in Python can be drawn using sns.barplot().

**2. Line Plot:** A single line plot presents data on the x-y axis using a line joining data points. To obtain a graph Seaborn comes with an inbuilt function to draw a line plot called line plot Line plot in python can be drawn using sns.lineplot().

**3. Box Plot:** Box plot is a visual representation of and comparison of groups of data. The box plot depicts the level, spread, and symmetry of a data distribution by using the median, approximate quartiles, outliers, and the lowest and highest data points (extreme values).

#### Multivariate GEDA

**1. Scatter plot:** Dots are used to indicate values for two different numeric variables in a scatter plot. The values for each data point are indicated by the position of each dot on the horizontal and vertical axes. Scatter plots are used to see how variables relate to one another. Here, scatter plot of the “Ladder score” against “Standard error of ladder score” is plotted.


**2. Heat Maps:** A heatmap is a graphical depiction of data that uses a color-coding method to represent various values. It represents a two- dimensional table of color- shades. This technique of plotting is popularly used in biology to represent gene expression and other multivariate data.

**3. Count Plot:** A Seaborn count plot is a graphical representation of the number of occurrences or frequency for each category data using bars to depict the number of occurrences or frequency. The countplot() function is used to visualize the number of observations in each categorical category as bars. Here, the Count plot is plotted for the subdata dataframe.

### Conclusion

In this paper, various phases of data analysis like cleaning, analysis but excluding data collection (given by AlmaBetter), are discussed briefly. Exploratory data analysis is mainly studied here. For the implementation, Python programming language is used. For detailed research, a colab notebook is used. Different Python libraries and packages are introduced. Using various analysis and visualization methods, numerous results are extracted. The dataset “Hotel Booking Analysis'' is used and extract important information like percentage of booking in City.






