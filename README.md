# Statistics Project with Python

# ✨ World's Happiness Score Dataset 

## 💎 The Aim Of The Project 
The main objective was to gain a deeper understanding of how 
statistical concepts are practically utilized in real-world contexts 
and to learn how to analyze and interpret a dataset. We were required 
to choose a dataset and perform calculations using the Python 
programming language to compute various statistics such as mean, 
standard error, and variance. By doing so, we aimed to bridge the gap 
between theoretical knowledge of statistics and its practical 
application in real-life situations.
<br><hr>
## 💎 What I Did in the Project
In the project, I chose the "World Happiness Score" dataset as the 
dataset. It includes the happiness scores of countries from 2015 to 
2019. My goal was to compare the happiness scores of specific countries 
by taking the last two years. First, I determined the countries I 
would select and kept them in a list. I read the happiness scores of 
these countries from the CSV file and stored them in a list. 
Additionally, to investigate whether the level of economic prosperity 
of the countries affects their happiness, I also kept the GDP values 
in a list. The function lengthOfList returns the length of a list. 
sumOfList calculates the sum of numbers in a list. In the findMean
function, I divided the sumOfList by the lengthOfList to find the 
mean. To find the median, I first sort my list with the sorted
function. If my list is even in length, I return the average of the 
middle two elements. If it's an odd number, I'm returning the middle 
element. In calculateVariance I am using a loop to calculate the 
squared difference between each element in the array and the mean, and 
I accumulate these squared differences in the variable 'sqDiff'. 
Finally, I divide the sum of squared differences by the size of the 
array to calculate the variance. In standartDeviation I returned the 
square root of the variance value. I also used the standardError
function to calculate the error rate. I divided the standard deviation 
by the square root of the sample size and returned the result. In 
removeOutliers; a z-score is computed for each value in the data array 
to determine its position relative to the mean in terms of standard 
deviations. The z-score measures the number of standard deviations a 
value deviates from the mean. Values that have a z-score greater than 
or less than a specific threshold value (usually set to 1 by default) 
are considered outliers. These outliers are identified and added to a 
separate list called 'outliers'. In confidenceInterval; 
to estimate the confidence interval, I select a sufficient sample size 
from the list and calculate its mean and standard deviation. Then, I 
calculate the t value using the t.ppf() function to achieve a 95% 
confidence level. By using the t score, I account for the small size 
of our dataset, which is recommended for accurate results. Finally, I 
compute the lower and upper limit values for the confidence interval 
based on the calculated t value, mean, standard deviation, and sample 
size. In the calculateSampleSize function, I first calculate the alpha 
value corresponding to the desired confidence level by subtracting the 
confidence level from 1. Then, using the norm.ppf() function from the 
library, I determine the z-score based on the alpha value. The z-score 
represents the percentile point value in the standard normal 
distribution, and it is chosen based on the desired confidence level 
and alpha value.
Next, I calculate the required sample size by multiplying the z-score 
by the standard deviation and dividing it by the specified margin 
value. The result is rounded to the nearest integer using the ceil()
function. This calculation gives an estimate of the sample size needed 
to achieve the desired confidence level and margin of error.
<br><hr>
