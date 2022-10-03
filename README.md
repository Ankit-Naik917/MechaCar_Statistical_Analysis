# MechaCar_Statistical_Analysis
## Linear Regression to Predict MPG

![Deliverable 1 Screenshot](https://user-images.githubusercontent.com/103617509/193675222-b4ebd0b2-9272-41bc-9dcf-7faabaeb7f55.png)

Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

Based on the output, it looks like "vehicle_length" and "ground_clearance" coefficiens provided a non random amount of variance to the mpg values in the dataset.

Is the slope of the linear model considered to be zero? Why or why not?

The slope of the linear model cannot be considered to be zero because the p-value is 5.35e^-11 is lower than extreme level of significance and therefore the null hypothesis must be rejected. Moreover, the coefficients of the variables are non-zero eventhought some of them are really close to zero. 

Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

The value of R-squared is 0.7149 which means that model has 71.5% accuracy in predicting the mpg of the MechCar prototypes. So this linear model effective enough to predict mpg of Mechacar prototypes.

## Summary Statistics on Suspension Coils

![Deliverable 2 Screenshot](https://user-images.githubusercontent.com/103617509/193675226-7b32c4e2-5379-4506-b5a9-9e0048a215ab.png)

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

The variance for total_summary screenshot above shows 62PSI which is below the design specification of 100PSI. Therefore we can say that the current manufacturing data meet the design specification for total manufacturing. However, when we look at the individual lots, the lot 1 and 2 are well within the specification but lot 3 is outside the specification with 170PSI variance. As a result, lot 3 does not meeting the specification. 

## T-Tests on Suspension Coils

![Deliverable 3 Screenshot](https://user-images.githubusercontent.com/103617509/193675229-b16cd446-bbe7-4e94-903e-1100b52c6d40.png)

summary of the t-test results across all manufacturing lots and for each lot

The total manufacturing mean value is 1498.78 which is close to the presumed mean of 1500. Moreover, the p-value is 0.0603 which is higher than the commonly accepted p-value of 0.05. There are no other evidence that is significant enough to support the rejection of null hypothesis. 

For Lot 1 and 2 the menas are 1500 and 1500.2 and p-values are 1 and 0.6072 respectively. There is no statistical difference between these means and the population mean and with the derived p-values we cannot reject the null hypothesis. However, in the case of lot 3, eventhough the mean is 1496.14 which show no statistical different between the population mean but the p-value is 0.0417 which is indicating that the null hypothesis should be rejected. 

## Study Design: MechaCar vs Competition

Write a short description of a statistical study that can quantify how the MechaCar performs against the competition. In your study design, think critically about what metrics would be of interest to a consumer: for a few examples, cost, city or highway fuel efficiency, horse power, maintenance cost, or safety rating. 

There are many matrics that consumer have interests before purchasing. I will consider safety rating, fuel type, highway/city fuel efficiency, horsepower and purchase price. 

The null hypothesis : the car is prices correctly based on the matrices.
The alternate hypothesis : the car is not priced based on the matrices.

Safety rating, fuel type, highway/city fuel efficiency and horsepower would be independant variable and purchase price would be dependent variable. Based on the variables mentioned, multiple linear regression test would be used to test the hypothesis due to the dependencis of purchase price on the independant variables.

To run the statistical test, we would require safety rating, fuel type, highway/city fuel efficiency, horsepower and purchase price data from mechacar dataset as well as same data from other competitors.
