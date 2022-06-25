# MechaCar_Statistical_Analysis


# Overview of Project

A few weeks after starting his new role, Jeremy is approached by upper management about a special project. AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team.


## Linear Regression to Predict MPG


![Linear_regression_summary](https://user-images.githubusercontent.com/101373142/175792554-778361d0-9b70-4a87-8f64-c53cdcf6b646.png)



The summary for a multiple linear regression using all the information from the MechaCar MPG data, we can see that vehicle length and ground clearance are strongly correlated with MPG.  Vehicle weight is also less correlated.  Evidenced by the larger coefficients for the significantly correlated factors, length and ground clearance, the Linear model has a non-zero slope. With an r2 of 0.715, this linear model predicts the MPG of the MechaCar prototypes effectively although given some of the insignificant variables included, it may be slightly overfitted.



## Summary Statistics on Suspension Coils

![total_summary](https://user-images.githubusercontent.com/101373142/175792409-ac00401a-5959-41e3-8823-27ab79d1c235.png)


The design specifications for the MechaCar suspension coils indicate the variance of the suspension coils must not exceed 100 PSI.  According to the summary statistics for the suspension coil data, it would appear this is met across manufacturing lots.


![lot_summary](https://user-images.githubusercontent.com/101373142/175792419-f52a5296-47bc-451a-a0d7-7b152b14b2fe.png)


However, reviewing the statistics lot by lot, we see that lot 3 is producing almost all the variance in the data set with a variance in PSI of 170. This is not sustainable for long-term.


## T-Tests on Suspension Coils


![one_sample_t-test](https://user-images.githubusercontent.com/101373142/175792461-2cbf0e11-fa45-4840-9ac9-7881dc70d810.png)

When performing a t-test on the suspension coil data,  as a whole, we cannot conclude that the PSI across all manufacturing lots are statistically different from the population mean of 1,500 PSI.


![t-test_lot1](https://user-images.githubusercontent.com/101373142/175792475-d470dc41-6cb7-4273-8b08-1e291fa237ea.png)



![t-test_lot2](https://user-images.githubusercontent.com/101373142/175792479-f59603c8-a735-4ec5-9631-78c65a204722.png)



![t-test_lot3](https://user-images.githubusercontent.com/101373142/175792483-311622cb-a8cd-40de-95fa-900fd2156b6f.png)


However, when performing t-tests lot by lot, we can conclude that lot 3 is statistically different from the population mean of 1,500 PSI.




## Study Design: MechaCar vs Competition

MechaCar can gain an advantage on the competition if it can be marketed as ‘Safe, Economical and Environment Friendly’.  To facilitate this, a statistical study should be done to determine if this is the case. MechaCar and its competition can be grouped by their cost and then compared across three metrics: MPG, maintenance cost, and safety rating in three respective two-sample t-tests to show that the alternative hypothesis: MechaCar has a statistical difference in the mean of each metric compared to the competition, is true. Two-sample t-tests work best here since MechaCar would be working with two different data sets, its own information on its vehicles and data on the competition. Obtaining efficient data is key to the study since two-sample t-tests contain reasonably large sample sizes and normally distributed data. For MechaCar's own data, this should be relatively straight forward. Obtaining reliable data from the competition should be the next step.
