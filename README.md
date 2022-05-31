# Data Analysis 8 - Simple Linear Regression
## Part 1 – ANOVA (10.5 points)
The General Social Survey collects data on demographics, education, and work, among many other characteristics of US residents. Using ANOVA, we can consider educational attainment levels for all 1,172 respondents at once. Below are the distributions of hours worked by educational attainment and relevant summary statistics that will be helpful in carrying out this analysis. 
1. (2 points) Write the null and alternative hypotheses for evaluating whether the average number of hours worked varies across the five groups.
2. Using the information provided, assess whether the following conditions necessary to accurately perform an ANOVA F test are met:
    - (0.5 point) Are the observations in the study independent?
    - (0.5 point) Are the sample sizes sufficiently large? (Hint: the n row of the table above provides the sample sizes of each group.)
    - (0.5 point) Is the variation in the groups about equal from one group to the next? (Hint: use the spread of the boxplots and standard deviation values from the table to assess this condition.)
3. To assess whether there is a significant difference in the average number of hours worked between one or more of the groups, we need to determine the mean squares between groups (MSG) and the mean squares within groups (MSE). Each of these values has an associated degrees of freedom. 
    - (1 point) Determine the degrees of freedom associated with the MSG. 
    - (1 point) Determine the degrees of freedom associated with the MSE. 
4. (1 point) An ANOVA was performed in R. The estimate for the mean squares between groups is MSG = 501.54 and the resulting F statistic is equal to 2.189. Determine the average variation within each group. That is, calculate the MSE. 
5. (2 points) Using the F statistic from question 4 and the two values for the degrees of freedom in question 3, calculate the p-value for this test. 
6. (2 points) Using the p-value calculated in question 5, write a conclusion for this ANOVA F test. (Hint: your conclusion should include a statement of evidence in favor of the alternative and a statement as to whether the null hypothesis is rejected or not.)

## Part 2 – Simple Linear Regression (12.5 points) 
In this lab we’ll be looking at data from all 30 Major League Baseball teams in 2011 and examining the linear relationship between runs scored in a season and the number of at-bats for each time. Our aim will be to summarize this relationship both graphically and numerically in order to determine if the number of at-bats helps us predict a team’s runs scored in a season.

For this part of the assignment, please refer to the DA8_ SLR.R script and the mlb.csv file available on the Canvas page for this assignment. Be sure to read through all comments in the R script to understand how we visualize and fit the least squares regression line in R. 

1. (1 point) We are interested in determining if the number of at-bats is a good predictor of the number of runs a team scores in the 2011 season. Identify the explanatory and response variables for this question of interest. 
2. (2.5 points) Using the R script, construct a scatterplot of the at-bat and runs variables. Paste your plot below. Using the scatterplot, describe the relationship between the number of at-bats and runs. Include the strength, direction, and form of the relationship. Comment on whether or not there are any outliers present in the data.  
3. (0.5 points) Calculate and report the correlation coefficient between the two quantitative variables. 
4. (2 points) Using the lm() and summary() functions provided to you in the R script, fit the least squares regression line that models the linear relationship between the number of at-bats and the number of runs scored. Write out the estimated least squares regression model. (Hint: your answer should be in the form  where  and  are replaced with the estimates for the intercept and slope.
5. (1 point) Interpret the slope estimate in the context of the problem. 
6. Using the R script, construct a plot of the residuals for this model. 
    - (1 point) Paste your residual plot below. 
    - (1.5 points) Use the residual plot to assess whether the conditions are met: linearity, normality in the response values, and constant variance about the regression line. Comment on whether or not you think each of these conditions are met and use the residual plot to support your comments. 
7. (1 point) Suppose a team expects 5,600 at-bats in one season. Use the least squares regression line you reported in question 4 to predict the number of runs the team will score. 
8. (1 point) Suppose the team in question 7 actually scores 728 runs in the season. Compute the residual for this team. 
9. (1 point) Now suppose that a new team is joining the MLB and only expects 4,900 at-bats in the season. Why is inappropriate to use this model to predict this team’s runs scored? 
