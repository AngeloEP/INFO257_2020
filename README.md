# INFO257_2020
Development of tasks subject INFO2020

## Key Concepts
**Training data** : The original data.

**Testing data** : Is data that we use to compare the predictions made by the fit model, we also use them to evaluate Machine Learning methods.

Note: Fitting the Training Data well but making poor predictions, is called the Bias-Variance Tradeoff.

- **Linear Regression:**
	- Use least-squares to fit a line to the data.
		* a) Draw a line through the data.
		* b) Measure the distance from the line to the data, square each distance, and then add them up(Residual).
		* c) Rotate the line a little bit.
		* d) Repeat the previous points until found you  the smallest sum of squared residuals.
		* d) Compare the results with their corresponding rotations. Then find the rotation that has the least sum of squares.
	- Calculate R².
		* This is done to find out how well the line fits the data.
		* a) Calculate the average of the variable to be predicted.
		* b) Move all data points to the y-axis.
		* c) Draw a black line to show the average of the variable to be predicted.
		* d) Now, sum the squared residuals(we'll call this SS(mean), for "sum of squares around the mean".
		* Note: SS(mean) = (data - mean)².
		* Note: Variation around the mean = (data - mean)² / n(sample size).
		* Note: SS(fit) = (data - line)².
		* Note: Variation around the line = (data - line)² / n(sample size).
		* Note: R² tells us how much of the variation of the dependent variable can be explained by taking explanatory variable into account .
		* R² = ( var(mean) - Var(fit) ) / var(mean).
		* Note: Also, R² = ( SS(mean) - SS(fit) ) / SS(mean).
		* Note: If R² = 0.6 = 60%, that is to say, 60% of the sums of squares of the dependent variable can be explained by explanatory variable.
	- Calculate a p-value for R².
		* This determines whether the R² value is statistically significant.
		* F = ( ( SS(mean) - SS(fit) ) / (rho_fit - rho_mean) ) / ( SS(fit) / (n - rho_fit) )

