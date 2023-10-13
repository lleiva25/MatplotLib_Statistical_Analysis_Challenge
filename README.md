# MatplotLib_Statistical_Analysis_Challenge

--------------------------------------------------------------------------------------------------------
Summary
--------------------------------------------------------------------------------------------------------
+ You've just joined Pymaceuticals, Inc., a new pharmaceutical company that specializes in anti-cancer medications. Recently, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.
As a senior data analyst at the company, you've been given access to the complete data from their most recent animal study. In this study, 249 mice who were identified with SCC tumors received treatment with a range of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens.
The executive team has tasked you with generating all of the tables and figures needed for the technical report of the clinical study. They have also asked you for a top-level summary of the study results.
--------------------------------------------------------------------------------------------------------
Data Analysis
--------------------------------------------------------------------------------------------------------
+ The drug regimen with the most mice participents are Capomulin and Ramicane.
+ The sex distribution of Male : Female are approximately the same with the percentages being 49.4% and 50.6% respectively.
+ Looking at the box plot comparing "Final Tumor Volume (mm3)" amongst the drugs, we can see that Capomulin and Ramicane had the lowest range for the final tumor volume compared to the others. This could mean that these drugs are more efficitive at treating tumors compared to the others. In addition, the only drug that had any outliers was Infubinol.
+ Supporting evidence of Capomulin being a very effictive drug is shown through the plot graph of "Tumor Volume (mm3)" vs "Timepoint". The initial tumor size has gone down significantly over time.
+ In addition, there seems to be a significant positive correlation between "Weight(g)" and "Tumor Volume (mm3)" due to the correlation coefficient being 0.84.
--------------------------------------------------------------------------------------------------------
Instructions
--------------------------------------------------------------------------------------------------------
Project overview:
+ Prepare the data.
+ Generate summary statistics.
+ Create bar charts and pie charts.
+ Calculate quartiles, find outliers, and create a box plot.
+ Create a line plot and a scatter plot.
+ Calculate correlation and regression.
+ Submit your final analysis.
+ Prepare the Data

Instructions:
+ Run the provided package dependency and data imports, and then merge the mouse_metadata and study_results DataFrames into a single DataFrame.
+ Display the number of unique mice IDs in the data, and then check for any mouse ID with duplicate time points. Display the data associated with that mouse ID, and then create a new DataFrame where this data is removed. Use this cleaned DataFrame for the remaining steps.
+ Display the updated number of unique mice IDs.
+ Generate Summary Statistics
+ Create a DataFrame of summary statistics. Remember, there is more than one method to produce the results you're after, so the method you use is less important than the result.


Statistical Analysis Data:
+ A row for each drug regimen. These regimen names should be contained in the index column.
+ A column for each of the following statistics: mean, median, variance, standard deviation, and SEM of the tumor volume.
+ Calculate Quartiles, and Find Outliers
  
Required Graphs:
+ Create Bar Charts and Pie Charts
+ Generate two bar charts. Both charts should be identical and show the total total number of rows (Mouse ID/Timepoints) for each drug regimen throughout the study.
+ Create the first bar chart with the Pandas DataFrame.plot() method.
+ Create the second bar chart with Matplotlib's pyplot methods.
+ Generate two pie charts. Both charts should be identical and show the distribution of female versus male mice in the study.
+ Create the first pie chart with the Pandas DataFrame.plot() method.
+ Create the second pie chart with Matplotlib's pyplot methods.
+ Create a Box Plot using the calculated quartiles and outliers.

Further Analysis:
+ Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then, calculate the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens. Use the following substeps:
+ Create a grouped DataFrame that shows the last (greatest) time point for each mouse. Merge this grouped DataFrame with the original cleaned DataFrame.
+ Create a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.
+ Loop through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment. Append the resulting final tumor volumes for each drug to the empty list.
+ Determine outliers by using the upper and lower bounds, and then print the results.
+ Using Matplotlib, generate a box plot that shows the distribution of the final tumor volume for all the mice in each treatment group. Highlight any potential outliers in the plot by changing their color and style.
