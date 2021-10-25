# MechaCar_Statistical_Analysis.
## Overview of the Project.
- Using R to provide visualizations, statistical tests, and interpretations of a large dataset.

## Linear Regression to Predict MPG.
- Performed a linear regression analysis which predicted the mpg of MechaCar prototypes using data from a csv file. The analysis can be viewed below:
![Linear Regression](https://user-images.githubusercontent.com/85714314/138744279-06c0b1f4-51e2-491f-8ce1-a80155e659d7.png)

- **Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?** From the model, the vehicle length and the ground_clearance provided non-random amoundts of variance to the mpg values.
- **Is the slope of the linear model considered to be zero? Why or why not?** The slope of the model is not considered to be zero. The p-Value is 5.35e-11 which is significantly smaller than the significance level of 0.05.
- **Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?** The model effectively predicts the mpg of MechaCar prototypes. The r value is 0.7149 which means there is a strong correlation determined.

# Suspension Coils Statistical Summary. 
- Performed a statistical analysis to determine whether the weight capacities of multiple suspension coils were consistent with production lots. 

**Total Summary**

![total_summary](https://user-images.githubusercontent.com/85714314/138746583-93e8cf7d-111e-4ea6-930b-8fd017df7183.png)

**Per Lot Summary**

![lot_summary](https://user-images.githubusercontent.com/85714314/138746707-c0797376-6b53-47f1-8dc9-cb587bf27e7e.png)

- **The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?**
According to the results, Lot 1 meets the design specifications best with a variance of 0.97. Lot 2 has a variance of 7.47, which is means the median and mean values are not significantly different and can meet design specifications. However the variance in lot 3 is 170.28, this does not meet design specifications. 

## T-test on Suspension Coils.
- T-tests were performed to determine if there was a statistical difference in the dataset. The population sample had a mean of 1500.

**All Lots Summary**

![t-test for all](https://user-images.githubusercontent.com/85714314/138748014-834e137e-6b70-4b75-a911-3de734f02d89.png)

- From the results, the p-Value is 0.06028, this is not enough evidence to reject the null hypothesis since it is higher than the normal significance of 0.05.

**Per Lot Summary**

![lot123](https://user-images.githubusercontent.com/85714314/138748307-e420337d-7fbb-400b-b372-14e11932b2dd.png)

- Per the results, lot 1 and 2 had p-Values of 1 and 0.60 respectively. For this lots, there was not enough evidence to reject the null hypotheis as the p-Values were higher than the significance of 0.05. However, Lot 3 had a p-Value of 0.042 which is lower than the normal significance, this indicates that the null hypotheis was rejected and the smaple mean and presumed population mean are not statistically different. 

## Study Design: MechaCar vs Competition.
- **Study** I have designed a statistical study in order to determine how MechaCar vehicles perform against vehicles made by other manufacturers. Potential metrics that consumers and investors would be interested in would be cost, highway efficiency(mpg) and fuel type(electric vs gas).

- **Hypothesis** Are MechaCar vehicles adequately priced in comparison to their competitors in terms of highway efficiency and fuel type?
- **Statistical Tests** Conducting a  two-sample t-test should be used to compare the distribution of both groups. Then performing one-tailed t-tests in order to determine which means are greater than or less than the other.
- **What data is needed to run the statistical test?** We would need to have data from both MechaCar and its competitors providing the metrics needed above and large sample data to extract statistical data from.





