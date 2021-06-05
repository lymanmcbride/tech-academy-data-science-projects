# Regression Assignment
## Introduction
The assignment is to write a linear regression for the data. This is bi-variate data, the independent variable is minutes running for the week, and the dependent variable is weight by week. Below I break down the math used to arrive at my equasion for a line of best fit
## Step 1: Extend the Table
- I calculated the mean of x (x̄) and the mean of y (ȳ) and placed them below the table
- I added 5 rows to the table on which I would perform various calculations for each row of data. 
    - The first row is the Standard Deviation of X (x-x̄)
    - The Second row is the Standard Deviation of Y (y-ȳ)
    - The third row is those standard deviations multiplied together
    - The fourth row is the first row squared
    - The fifth row is the second row squared
- At the bottom of the 3-5th rows I summed each column

## Step 2: Calculate Correlation Coefficient
- Using my calculations from the table, I calculated the correlation coefficient using the formula. 
- Sum of Standard Deviations divided by the square root of the sum of the X standard deviations squared times the sum of the Y standard deviations squared. 
- Put simply: F11/SquareRoot(G11*H11)

## Step 3: Find The Standard Deviations of X and Y
- Take the Square Root of the Sum of the squared individual standard deviations divided by the number of data points minus 1
- simply: SquareRoot(G11/numberOfDataPoints-1)
- Do the same as above but for Y:
    - SquareRoot(H11/numberOfDataPoints-1)

## Step 4: Find Slope
- Slope is the Correlation Coefficient times the Standard Deviation of Y over the standard deviation of X
- Using the calculations above, I just had to put certain cells into that equastion: C14*(C16/C15)

## Step 5: Find Y Intercept
- Y Intercept can be found by taking the mean of Y minus the slope times the mean of X
- C12-C17*B12

## Step 6: Write out the equasion
- Using everything above, you can now write Y=Slope times X plus Y intercept
- y = .042x + 175.57

