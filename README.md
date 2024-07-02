# data-visualization-challenge

Study to compare the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens.

[Analysis](https://github.com/caitlin-hartley/data-visualization-challenge/blob/main/README.md#analysis)

## Prepare the Data

  - Merge the mouse_metadata and study_results DataFrames into a single DataFrame
  - Display the number of unique mice IDs in the data
  - Check for any mouse ID with duplicate time points
  - Create new clean DataFrame where duplicate mouse is removed

![merge](https://github.com/caitlin-hartley/data-visualization-challenge/blob/main/images/merge_data.png)

![clean](https://github.com/caitlin-hartley/data-visualization-challenge/blob/main/images/clean_data.png)

## Generate Summary Statistics

  - Generate summary statistic table including: mean, median, variance, standard deviation, and SEM of the tumor volume.

![summary](https://github.com/caitlin-hartley/data-visualization-challenge/blob/main/images/summary_stats.png)

## Create Bar Charts and Pie Charts

  - Generate two bar charts that show the total total number of rows (Mouse ID/Timepoints) for each drug regimen throughout the study
  - Generate two pie charts that show the distribution of female versus male mice in the study

![bar](https://github.com/caitlin-hartley/data-visualization-challenge/blob/main/images/bar_plot.png)

![pie](https://github.com/caitlin-hartley/data-visualization-challenge/blob/main/images/pie_chart.png)

## Calculate Quartiles, Find Outliers, and Create a Box Plot

  - Calculate the final tumor volume of each mouse across four regimens: Capomulin, Ramicane, Infubinol, and Ceftamin
  - Calculate the quartiles and IQR, and determine if there are any potential outliers
  - Create a list for treatment names and an empty list to hold the tumor volume data
  - Loop through each drug in the treatment list and append the resulting final tumor volumes for each drug to the empty list
  - Determine outliers by using the upper and lower bounds
  - Generate a box plot that shows the distribution of the final tumor volume for all the mice in each treatment group

![quartiles](https://github.com/caitlin-hartley/data-visualization-challenge/blob/main/images/quartiles_outliers.png)

![box](https://github.com/caitlin-hartley/data-visualization-challenge/blob/main/images/box_whisker.png)

## Create a Line Plot and a Scatter Plot

  - Select single mouse that was treated with Capomulin
  - Generate a line plot of tumor volume versus time point for that mouse

![line](https://github.com/caitlin-hartley/data-visualization-challenge/blob/main/images/line.png)

![scatter](https://github.com/caitlin-hartley/data-visualization-challenge/blob/main/images/scatter.png)

## Calculate Correlation and Regression

  - Calculate the correlation coefficient and linear regression model between mouse weight and average observed tumor volume for the Capomulin treatment regimen
  - Plot the linear regression model

![correlation](https://github.com/caitlin-hartley/data-visualization-challenge/blob/main/images/correlation.png)

## Analysis

  - Based on the data, Capomulin and Ramicane are the most effective treatments. The average tumor volume and final tumor volume for both of these treatments is significanly less than the other treatments. Additionally, the mice using these treatments have the highest number of observed timepoints, indicating the mice given these treatments potentially live longer.
  - The data also shows a strong correlation between mouse weight and average tumor size for the Capomulin regimine, with a correlation coefficient of 0.84. 
