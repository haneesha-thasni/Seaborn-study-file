![image](https://github.com/user-attachments/assets/f22b1fa5-769f-4ae5-b0b0-fef82f429710)

Visualization is an important part of storytelling, we can gain a lot of information from data by simply just plotting the features of data. Python provides a numerous number of libraries for data visualization.
## What is Seaborn
Seaborn is an amazing visualization library for statistical graphics plotting in Python. It provides beautiful default styles and color palettes to make statistical plots more attractive. It is built on top matplotlib library and is also closely integrated with the data structures from pandas.
Seaborn aims to make visualization the central part of exploring and understanding data. It provides dataset-oriented APIs so that we can switch between different visual representations for the same variables for a better understanding of the dataset.
## Different categories of plot in Seaborn 
Plots are basically used for visualizing the relationship between variables. Those variables can be either completely numerical or a category like a group, class, or division. Seaborn divides the plot into the below categories – 

* Relational plots: This plot is used to understand the relation between two variables.
* Categorical plots: This plot deals with categorical variables and how they can be visualized.
* Distribution plots: This plot is used for examining univariate and bivariate distributions
* Regression plots: The regression plots in Seaborn are primarily intended to add a visual guide that helps to emphasize patterns in a dataset during exploratory data analyses.
* Matrix plots: A matrix plot is an array of scatterplots.
* Multi-plot grids: It is a useful approach to draw multiple instances of the same plot on different subsets of the dataset.
## Installation of Seaborn Library 
For Python environment : 

    pip install seaborn
For conda environment : 

    conda install seaborn
## Import seaborn
Import the Seaborn module in your code using the following statement:
     
     import seaborn as sns
## Common Plots in seaborn
![image](https://github.com/user-attachments/assets/af4d7271-aa25-4c02-913a-dc9e0dffc4f4)

1. Bar Plots
2. Count Plots
3. Histograms
4. Cat Plots (Box, Violin, Swarm, Boxen)
5. Multiple Plots using FacetGrid
6. Joint Plots
7. KDE Plots
8. Pairplots
9. Heatmaps
10. Scatter Plots

### 1. Bar Plots
* Bar plots can be used to visualize various types of data, such as counts, frequencies, percentages, or averages.
* They are particularly useful for displaying and comparing data from different categories.
#### Use Cases:
  - Categorical Comparison: Each bar represents a distinct category, and the height of the bar indicates the aggregated value associated with that category (count, sum or mean).
  - Proportional Representation through Stacked Bar Charts: Bar plots can also represent proportions or percentages. By scaling the height of each bar to represent the proportion of observations in a category, it is possible to compare the relative distribution of different categories.
  - Comparison of Subcategories within each category through Clustered Bar Plots: Multiple bars can be grouped within each category to represent different subcategories, allowing for comparison and analysis.
### 2. Count Plots
* A count plot displays the number of occurrences of each category in a categorical variable.
* The x-axis represents the categories of the variable, while the y-axis represents the count or frequency of each category.
#### Use Cases:
  - Frequency Distribution of categorical variables: Each bar represents a category, and the height of the bar represents the frequency or count of observations in that category. This helps to identify the most common or least common categories.
  - Relationship between different categorical variables.
### 3. Histograms
* Histograms are graphical representations of the distribution of a dataset.
* They can reveal important characteristics of the data, such as whether it follows a normal distribution, is skewed to one side, or has multiple peaks.
* They display the frequency or count of observations within different intervals or “bins” of the data.
* The x-axis of a histogram represents the range of values in the dataset, divided into equally spaced intervals or bins.
* The y-axis represents the frequency or count of observations falling within each bin.
* The height of each bar in the histogram corresponds to the number of observations in that bin.
#### Use Cases:
   - Visualize the shape, centre, range and spread of a continuous/numeric variable and to identify any patterns or outliers.
   - Compare the distribution of many continuous variables.
   - Compare the distribution of a continuous variable for different categories.
### 4. Cat Plots (Box, Violin, Swarm, Boxen)
* Catplot is a higher-level versatile function that combines several underlying categorical seaborn plots like boxplots, violinplots, swarmplots, pointplots, barplots and countplots.
#### Use Cases:
   - Explore relationship between categorical and a continuous variables.
   - Get the statistical summary of a continuous variable.
### 5. Multiple Plots using FacetGrid
* FacetGrid is a feature in the seaborn library that allows you to create multiple subsets of your data in a grid-like arrangement.
* You can create a grid of plots where each plot represents a category.
* The subsets are determined by the column names given in the ‘col’ and ‘row’ attribute of FacetGrid().
* The individual plots within the grid can be any type of plot supported by seaborn, such as scatter plots, line plots, bar plots, or histograms.
#### Use Cases:
   - Compare and analyse different groups or categories within your dataset.
   - Create subplots seamlessly.
### 6. Joint Plots
* A joint plot combines multiple univariate and bivariate plots in a single figure.
* The central plot typically displays a scatter plot or a hexbin plot, representing the joint distribution of the two variables.
* This main plot is accompanied by additional plots along the axes (histograms or KDEs) that show the distributions of each variable individually.
#### Use Cases:
   - Finding the relationship between 2 variables.
   - Comparing the individual distributions of 2 different variables.
### 7. KDE Plots
* A KDE (Kernel Density Estimate) plot is a smoothed version of a histogram representing the probability density function of a continuous random variable.
* The y-axis represents the density or likelihood of observing a particular value of the variable, and the x-axis represents the values of the variable itself.
#### Use cases:
  - visualization of the distribution of a single variable (univariate analysis).
  - Insights into the shape, peaks, and skewness of the distribution.
### 8. Pairplots
* A pair plot is a type of visualization that allows you to explore the relationships between multiple variables in a dataset.
* It is a grid of scatter plots, where each variable is plotted against every other variable.
* In a pair plot, the diagonal entries are histograms or density plots for each variable, showing the distribution of values.
#### Use Cases:
  - Identification of correlations or patterns between variables, such as linear or non-linear relationships, clusters, or outliers.
### 9. Heatmaps
* Heatmaps are a type of visual representation that use color-coded cells to display the values of a matrix or a table of data.
* In a heatmap, the rows and columns of the matrix represent two different variables, and the color intensity of each cell represents the value or magnitude of the data point at the intersection of those variables.
#### Use Cases:
  - Correlation analysis, visualisation of pivot tables which aggragate data by rows and columns.
### 10. Scatter Plots
* A scatterplot displays the relationship between two continuous variables.
* It is constructed by plotting individual data points on a graph with one variable represented on the x-axis and the other variable represented on the y-axis.
* The resulting plot consists of multiple points scattered across the graph, hence the name “scatterplot.”
#### Use Cases:
  - Relationship Assessment: Scatterplots help determine the nature of the relationship between two continuous variables. It can reveal if there is a positive correlation (both variables increase or decrease together), negative correlation (one variable increases while the other decreases), or no correlation (no apparent relationship).
  - Outlier Identification: Scatterplots can highlight outliers, which are data points that deviate significantly from the overall pattern.
  - Clustering and Grouping: By visually examining the distribution of points, you can identify if there are natural groupings or patterns among the variables.
  - Trend Analysis: By plotting data points chronologically, scatterplots can depict the evolution or progression of variables, helping to identify trends or changes in behaviour.
  - Model Validation: By comparing the predicted values of a model to the actual values, scatterplots can visualize the accuracy or deviation of the model’s predictions.
  

