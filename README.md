# MechaCar_Statistical_Analysis
# Deliverable 1:
Linear Regression to Predict MPG
Deliverable Requirements:
The MechaCar_mpg.csv dataset contains mpg test results for 50 prototype MechaCars. The MechaCar prototypes were produced using multiple design specifications to identify ideal vehicle performance. Multiple metrics, such as vehicle length, vehicle weight, spoiler angle, drivetrain, and ground clearance, were collected for each vehicle. Using your knowledge of R, you’ll design a linear model that predicts the mpg of MechaCar prototypes using several variables from the MechaCar_mpg.csv file.

To Deliver.

The MechaCar_mpg.csv file is imported and read into a dataframe
An RScript is written for a linear regression model to be performed on all six variables
An RScript is written to create the statistical summary of the linear regression model with the intended p-values
There is a summary that addresses all three questions
Results on Deliverable:
Resulting Model:

mpg = (6.267)vehicle_length + (0.0012)vehicle_weight + (0.0688)spoiler_angle + (3.546)ground_clearance + (-3.411)AWD + (-104.0)
![image](https://user-images.githubusercontent.com/95143562/162961521-71a442ee-6939-47c6-b5dd-e8d1730ce595.png)

From the above output we can see that:

1. The vehicle length, and vehicle ground clearance are statistically likely to provide non-random amounts of variance to the model. That is to say, the vehicle length and vehicle ground clearance have a significant impact on miles per gallon on the MechaCar prototype. Conversely, the vehicle weight, spoiler angle, and All Wheel Drive (AWD) have p-Values that indicate a random amount of variance with the dataset.

2. The p-Value for this model, p-Value: 5.35e-11, is much smaller than the assumed significance level of 0.05%. This indicates there is sufficient evidence to reject our null hypothesis, which further indcates that the slope of this linear model is not zero.

3. This linear model has an r-squared value of 0.7149, which means that approximately 71% of all mpg predictions will be determined by this model. Relatively speaking, his multiple regression model does predict mpg of MechaCar prototypes effectively.

If we remove the less impactful independent variables (vehicle weight, spoiler angle, and All Wheel Drive), the predictability does decrease, but not drastically: the r-squared value falls from 0.7149 to 0.674.

![image](https://user-images.githubusercontent.com/95143562/162961729-41fd4a13-71bd-491b-8dea-7f8544e49da4.png)


# Deliverable 2:
Summary Statistics on Suspension Coils
Deliverable Requirements:
The MechaCar Suspension_Coil.csv dataset contains the results from multiple production lots. In this dataset, the weight capacities of multiple suspension coils were tested to determine if the manufacturing process is consistent across production lots. Using your knowledge of R, you’ll create a summary statistics table to show:

The suspension coil’s PSI continuous variable across all manufacturing lots
The following PSI metrics for each lot: mean, median, variance, and standard deviation.
Technical Analysis
1. Download the Suspension_Coil.csv file, and place it in the active directory for your R session.
2. In your MechaCarChallenge.RScript, import and read in the Suspension_Coil.csv file as a table.
3. Write an RScript that creates a total_summary dataframe using the summarize() function to get the mean, median, variance, and standard deviation of the suspension coil’s PSI column.
Your total_summary dataframe should look like this:
![image](https://user-images.githubusercontent.com/95143562/162961854-98a48a8e-f089-4195-849a-1c8900688c90.png)

4. Write an RScript that creates a lot_summary dataframe using the group_by() and the summarize() functions to group each manufacturing lot by the mean, median, variance, and standard deviation of the suspension coil’s PSI column. Your lot_summary dataframe should look like this:
![image](https://user-images.githubusercontent.com/95143562/162961977-65744f02-7a5e-420e-8c10-46d5600f77a2.png)

5. Save your MechaCarChallenge.RScript file to your GitHub repository.
To Deliver.

You will earn a perfect score for Deliverable 2 by completing all requirements below:

The Suspension_Coil.csv file is imported and read into a dataframe
An RScript is written to create a total summary dataframe that has the mean, median, variance, and standard deviation of the PSI for all manufacturing lots
An RScript is written to create a lot summary dataframe that has the mean, median, variance, and standard deviation for each manufacturing lot
There is a summary that addresses the design specification requirement for all the manufacturing lots and each lot individually
The Suspension Coil dataset provided for the MechaCar contains the results of testing the weight capacities of multiple suspension coils from multiple production lots to determine consistency.

