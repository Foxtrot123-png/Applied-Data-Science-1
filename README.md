#Project Overview
This project provides a detailed analysis of user behavior data from a mobile app usage dataset, user_behavior_dataset.csv.
This dataset contains the data of users with their behavioural category they fall into. We would be comparing the user data to study what affects the behavioural category the user falls into and predict what the characteristics of a High Engagement user and Low engagement user look like. We would be taking help of Pascal Correlation to find the correlation between the numerical data and graphs such as a Histogram, Bar Chart, Box Plot and Scatter Plot.

#Dataset Description
The dataset contains the following fields:

User ID: Unique identifier for each user.
Device Model: Model of the device used.
Operating System: OS used by the device (e.g., Android, iOS).
App Usage Time (min/day): Time spent on apps per day.
Screen On Time (hours/day): Total screen on time per day.
Battery Drain (mAh/day): Battery drain per day in mAh.
Number of Apps Installed: Number of apps installed on the device.
Data Usage (MB/day): Data consumption per day.
Age: Age of the user.
Gender: Gender of the user.
User Behavior Class: An integer classifying user engagement levels, ranging from 1 (low engagement) to 5 (very high engagement).

#Libraries Needed


LANGUAGE:
Python (3.12.7)

Libraries Needed:
Numpy
Pandas
matplotlib.pyplot
seaborn

Used As:
import numpy as np 
import pandas as pd 
import matplotlib.pyplot as plt
import seaborn as sns


#Function Description

plot_hist():

Creates a Histogram for the given Data 
Parameters:
    - data (dataset) : Dataframe we need to study containing the columns 
    - x_var (list or a array) : The data to plot.
    - title (str, optional) : The title of the plot.
    - xlabel (str, optional) : The label for x-axis.
    - ylabel (str, optional) : The label for y-axis.
    - bins (int ,optional) : The number of bins to divide the data into (Default is 5).
    - color (str, optional) : THe color of the bars (Default is lightblue).
    - edgecolour (str, optional) : The color of the bar edges (Default is black).
    - alpha (float,optional)The transparency of the bars, from 0 (transparent) to 1 (opaque) (default is 0.8).
Returns:
    - None: The function will display a Histogram

plot_barplot():

Creates a Bar Chart for the given Data 

Parameters:
    - data (dataset) : Dataframe we need to study containing the columns 
    - column_name (list or a array) : The data to plot.
    - title (str, optional) : The title of the plot.
    - xlabel (str, optional) : The label for x-axis.
    - ylabel (str, optional) : The label for y-axis.
    - color1 (str, optional) : Color of the 1st Bar (Default is Blue)
    - color2 (str, optional) : Color of the 1st red (Default is Red)

Returns:
    - None: The function will display a Bar Chart

plot_boxplot():

Creates a Box Plot for the given Data 

Parameters:
    - data (dataset) : Dataframe we need to study containing the columns 
    - xaxis (str) : The Column name to plot on x axis 
    - yaxis (str) : The column name to plot on y axis .
    - title (str, optional) : The title of the plot.
    - rotation_direction (str) : Direction in which the labels on x axis needs to be tilted(Values it can take ---).
    - xticklabelcolumnname (str) : Name of the columns to assign as a  values on the ticks on x-axis.
    - xlabel (str, optional) : The label for x-axis.
    - ylabel (str, optional) : The label for y-axis.
    - facecolor (str, optional) : The color inside the box (Default is lightblue)

Returns:
    - None: The function will display a Box Plot
    
plot_scatterplot():

Creates a Scatter Plot for the given Data 

Parameters:
    - data (dataset) : Dataframe we need to study containing the columns 
    - xaxis (str) : The Column name to plot on x axis 
    - yaxis (str) : The column name to plot on y axis .
    - title (str, optional) : The title of the plot.
    - hue (str or list) : Grouping variable that will produce points with different colors. Default is None
    - xlabel (str, optional) : The label for x-axis.
    - ylabel (str, optional) : The label for y-axis.
    - palette (str or list): Colors to use for different levels of the hue. 
    - alpha (float): Transparency of the points, between 0(fully transparent) and 1(fully opaque).
    - legend_title (str): Title for the legend.
    - location_of_title (str): Position of the title. Can be 'center', 'left', or 'right'.
    - fontsize (int, optional) : Fontsize of the legend (Default is 14)

Returns:
    - None: The function will display a Box Plot
