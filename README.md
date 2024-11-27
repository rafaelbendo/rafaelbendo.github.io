# ICESat-2 (AGU) - Meeting 11-27

# Map

The first thing to do is to make a Map of the path of the tracks.

![image](https://github.com/user-attachments/assets/8a98df37-f40e-4189-97d2-735a965d9cc0)

Then I made a zoom at the gt3 beam

![image](https://github.com/user-attachments/assets/163fc79b-ef15-40f0-b610-0cb72b4e1de3)

## LOWESS Regression

LOWESS (Locally Weighted Scatterplot Smoothing), also known as LOESS (Locally Estimated Scatterplot Smoothing), is a non-parametric regression technique used to fit a smooth curve through data points in a scatterplot. It is particularly useful for exploring relationships between variables when the data might not follow a linear or predefined functional form. 

![image](https://github.com/user-attachments/assets/ccc7277c-8716-44bf-a58b-cd3c40027cdb)

How it works?

![image](https://github.com/user-attachments/assets/0bfb1351-46a9-4031-9aa0-f717ae377e48)

![image](https://github.com/user-attachments/assets/085810e7-6138-48e1-8b22-33d2df3a9f6c)

![image](https://github.com/user-attachments/assets/9a13016a-d448-414d-9d0c-52443c3b3c56)

see: https://medium.com/p/f26e523d7a35

#How LOWESS Works
1. Local Fitting:
* Instead of fitting a single global regression model (like linear regression), LOWESS fits a separate regression for each point in the dataset.
* It uses nearby points (within a defined "neighborhood") to estimate the value of the regression line at that point.

2. Weighted Regression:
* Points closer to the target point (where the regression is being calculated) are given higher weights, while points farther away have lower weights.
* The weights typically follow a kernel function, such as a tricube weighting function.

3. Smoothing:
The degree of smoothing is controlled by a smoothing parameter or span (often called 
α
α).
A larger span means more points are included in each local regression, resulting in a smoother curve.
A smaller span results in a curve that follows the data more closely, potentially capturing noise.

# My samples to Lowess 
![Lowess1](https://github.com/user-attachments/assets/f9144b51-fb01-4263-a81c-0ebc2937856c)

![Lowess2](https://github.com/user-attachments/assets/33c3721a-16bb-4e7c-8a7e-adc3c631e5cd)

** This is not a final choice, I already need to work the lowess model **

## Results Plots

I did a plot for each ground track for ATL03 - Track 0129

# Plot with all lines

![gt2l_evo](https://github.com/user-attachments/assets/3da5bc66-11d5-49db-b5dd-d70d0bcfc780)

# Plot with lines for 2019 and 2024
174 meters of retreat! 

![gt2l](https://github.com/user-attachments/assets/d841ad19-c8f0-472f-9011-aee4dfb90504)

# gt2r

![gt2r](https://github.com/user-attachments/assets/cf8e9e08-622b-440f-8ccd-b7f71c144206)

#gt3l

![gt3l](https://github.com/user-attachments/assets/3091dcd0-e499-4859-b40b-257ceecfdcd8)

#gt3r

![gt3r](https://github.com/user-attachments/assets/74d65a18-131d-4c97-a342-369e1961139c)







