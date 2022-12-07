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


