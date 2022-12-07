# Statistical Analysis Overview

**Sheets Included:**
- Data Repository Table (Raw)
- DRT Rolling Mean
- DRT Rolling Stdev
- Regressive Analysis
- Data Preparation
- Descriptive Statistics*
- Inferential Statistics*
 
*= Notes in README file

# Descriptive Statistics
Q1. Create a line plot for all the variable(s) in the Data Repository Table where the Data Source is filtered to 'Raw', with the exception to this being the column labelled Pump Failure (1 or 0). Upon completion of this, list down what observation(s) you have noted from the time-series line plot. Are there any variables that seem to exhibit any irregular looking trends?
 
- The data occasionally jumps up and then drops suddenly towards the end.

Q2. Just as you did in Q1, create a line plot for all the variable(s) in the Data Repository Table - Raw Tab. However, this time, ensure that the Horse Power Variable and the Pump Failure (1 or 0) Variable is plotted on the secondary axes.What observations do you note when viewing the data in this way?

- There are multiple jumps or spikes in the data at certain intervals, with a sharp uptick in readings towards the end of the data series.

Q3. Just as you did in Q1 and Q2, create two line plots for all the variables in the DRT Rolling Stdev and DRT Rolling Mean Tabs. Ensure that the Horse Power variable and Pump Failure (1 or 0) are plotted on a secondary-axis. Note down what observations/trends emerge when you look at the data in this manner - are there any trends that are more pronounced with the Rolling Mean / Rolling Stdev data?

- The data fluctuations are a lot more noticeable, especially with the DRT Rolling Stdev data, and the sharp spike in number readings is even more dramatically pronounced in both graphs.

Q4. Using the data in columns C through to I for each of the three (3) Data Repository Table - Raw, DRT Rolling Stdev and DRT Rolling Mean Tabs, create Two Box Plots. The first box plot will be filtered to contain the Pump Failure Data when Pump Failure is equal to 1 (The pump has failed). The second box plot will be filtered to contain the Pump Failure Data when Pump Failure is Equal to 0 (i.e. The Pump has not yet failed).
You'll end up creating six (6) box plots, two for each dataset. Remember that when you change the Pump Failure Filter from 1 to 0, the Box Plots will automatically update so you will need to work out an approach to make sure the Box Plots retain either the Pump Failure = 1 or Pump Failure = 0 Data (Otherwise, your Box Plots may be skewed). What trends become apparent when viewing the data in this manner?

- There are noticeably larger median/mean values in the 2nd and 3rd quartiles for the "Pump Failure = 1" charts, and in most of the "Pump failure = 0" charts, the data appears to have a lot of extreme outliers in the first and fourth quartiles.

# Inferential Statistics

Q1.Using the three datasets in the Data Repository Tab (Raw, Rolling Mean (30 Minutes), Rolling Standard Deviation (30 Minutes)), create three separate correlation heatmaps. This can be completed using the Data-Analysis Add-In and selecting 'Correlation'. What do you observe about the correlations when focusing specifically on the 'Pump Failure (1 or 0)' Row? Note: It may be helpful to apply conditional formatting to make the correlation scores easier to interpret! (i.e. The closer to 1 is green, the closer to -1 is red)

- The Volumetric Flow Meters (1 and 2) and the Pump Efficiency categories appear to show the lowest values in regards to Pump Failure, indicating a possible correlation between low volumetric flow measurements and pump failure. 

Q6. For each of the three Correlation Heatmaps you have created, create THREE Column Charts using the Pump Failure (1 or 0) data (Row 23) and order this in descending order. 

- Looking at all three of our correlation heat-maps and associated correlation column plots, it is apparent that one of our three data-sets happens to show variables which are closely correlated with Pump Failure. (The Rolling Standard Deviation Dataset). However, this doesn't mean that our other datasets and correlations are not informative. The concept we are reinforcing here is that when looking at analysing time series data and events of interest, we should pay particularly strong attention towards variables which exhibit the largest degree of statistical variance. For example, we might note that a rapid increase in the Standard Deviation, seems to be a good indicator of failure.  


Q7. Using the Data Preparation Tab, create a multivariate linear regression. As you look at the Summary Output from the Linear Regression Model - what does the R Squared Value tell you about your model? What about the P-Value? Similar to what you had done with the correlation analysis in Q5, you just need to select 'Regression' from the Data Analysis Tab and put in the respective dependent and independent variables you wish to explore!

- Since the R-Squared value is below 0.4, it shows a very low level of correlation; whereas the P-values fluxuate dramatically, showing varying degrees of high correlation (Volumetric Flow Meters 1 & 2, Pump Temperature, etc.) and low correlation (Pump Speed, Pump Torque, etc.) depending on the variable being evaluated. 

Q8. Create the Multivariate Regression Equation Values for each row using the Regression Coefficients you have calculated in Q7. From your output, this will become the Statistical Alarm Signal that the Engineers will observe in the future for abnormalities. Place each co-efficient that you have calculated in the table titled 'Co-Efficients (Taken from the Summary Output Tab created when you calculate the Multivariate Regression)' in the Data Preparation Tab. What do you notice when you've completed your Multivariate Equation Plot? 

- There are fairly consistent and only slightly fluctuating measurements for the majority of the values. However there is a huge spike towards the end of the data set with the Pump Efficiency and Regressive Equation variables, and a smaller but still noticeable spike in the other variables as well, thus showing a possible correlation between Pump Efficiency and Pump Failure.

Q9. Revisiting the Regression Coefficients you have calculated in Q7, create a Column Chart that shows in descending order, each variables Regression Coefficient. Having completed this - what does this tell you about the variables that have the largest absolute impact towards Pump Failure? Additionally, how is this regression coefficient different from the correlation coefficient?

- Pump Speed, Pump Efficiency, and Pump Torque appear to have the strongest impact on Pump Failure. The regression coefficient shows how one variable affects another variable in a data set, whereas the correlation coefficient measures the numerical amount or linear relationship between two (or more) variables in a data set such as x and y. 

**Well done! We've managed to create a Statistical Alarm that the Engineers can look at and use to identify potential Pump Failure for the Surjek Asset!**
