**SENG 637- Dependability and Reliability of Software Systems\***

**Lab. Report \#5 – Software Reliability Assessment**

| Group \#:      |     |
| -------------- | --- |
| Student Names: |     |
|                |     |
|                |     |
|                |     |

# Introduction

#

# Assessment Using Reliability Growth Testing

## Screenshots

### MVF Plot of All Models & Covariates

![all_models_MVF_RGT](https://github.com/seng637-Winter/seng637-a5-Satchytan/blob/main/Screenshots/all_models_MVF_RGT.JPG "all_models_MVF_RGT")

### Intensity Graph of All Models & Covariates

![all_models_intensity_RGT](https://github.com/seng637-Winter/seng637-a5-Satchytan/blob/main/Screenshots/all_models_intensity_RGT.JPG "all_models_intensity_RGT")

### Tables for Comparison and Model Selection

![all_models_comparison_RGT.JPG](https://github.com/seng637-Winter/seng637-a5-Satchytan/blob/main/Screenshots/all_models_comparison_RGT.JPG "all_models_comparison_RGT.JPG")

![F_models_comparison_RGT.JPG](https://github.com/seng637-Winter/seng637-a5-Satchytan/blob/main/Screenshots/F_models_comparison_RGT.JPG "F_models_comparison_RGT.JPG")

![F_models_top2_RGT.JPG](https://github.com/seng637-Winter/seng637-a5-Satchytan/blob/main/Screenshots/F_models_top2_RGT.JPG "F_models_top2_RGT.JPG")

## Selection of Top 2 Models to Provide Best Fit

After analyzing the provided failure data and comparing various models with different covariates, our team identified Discrete Weibull (DW3) and Geometric (GM) models as the best fit for the project data using model ranking.

We used the following models for our comparison, IFR generalized Salvia & Bollinger, S Distribution, Discrete Weibull (Order 2), Discrete Weibull (Type III), Geometric, Negative Binomial (Order 2), and Truncated Logistic. We used Covariates E, F and C for our comparison, and found that covariate F produced the best AIC & BIC scores across all models. Therefore, for our direct model analysis and selection, we compared these scores to determine the selection of our 2 models. As shown in the screenshots below Discrete Weibull (DW3) and Geometric (GM) using covariate F yielded our best results, and so these 2 models are our selection for best model using Reliability Growth Testing.

| Model Name                                  | Covariate | AIC Score | BIC Score |
| ------------------------------------------- | --------- | --------- | --------- |
| IFR generalized Salvia & Bollinger {IFRGSB} | F         | 126.310   | 132.046   |
| S Distribution {S}                          | F         | 127.323   | 133.059   |
| Discrete Weibull (Order 2) {DW2}            | F         | 173.107   | 177.409   |
| Discrete Weibull (Type III) {DW3}           | F         | 122.199   | 127.935   |
| Geometric {GM}                              | F         | 125.323   | 129.625   |
| Negative Binomial (Order 2) {NB2}           | F         | 152.626   | 156.928   |
| Truncated Logistic {TL}                     | F         | 127.323   | 133.059   |

## Selection of Range of Useful Data

To determine the range of useful data for analysis, we conducted a visual inspection of the cumulative plot of failures over time. Upon examination, we observed that the initial time intervals exhibited a steep increase in failure count, indicating an 'infant mortality' phase where failure rates were high. This phase is typically associated with initial system setup, calibration, or early testing stages, where failures are more common due to initial defects or adjustments.

After interval 4, the plot displayed a more gradual increase in failure count, suggesting a period of relative stability in the system's performance. This stable phase is essential for reliable model fitting and analysis as it represents the system's behavior under more consistent operating conditions.

Therefore, we determined that the range of useful data for model fitting begins after interval 4. We excluded the initial 'infant mortality' phase and focused on the subsequent intervals where the system's performance stabilized. This approach ensures that our analysis captures data points that are representative of the system's reliability under typical operating conditions, leading to more accurate model selection and interpretation.

## Discussion of Acceptable Range of Failure Rate

In assessing the acceptable range of failure rate for the provided test data, several factors must be considered, including project requirements, safety standards, and industry norms.

Upon analysis of the failure data, we observed varying failure rates across different time intervals. It's important to note that failure rates can fluctuate due to factors such as system complexity, environmental conditions, and testing procedures.

For this specific dataset, the failure rate appears to be highest during the initial time intervals, corresponding to the 'infant mortality' phase. This is expected as the system undergoes initial testing and calibration, where defects and vulnerabilities are often identified and addressed.

As the testing progresses, we observe a decrease in the failure rate, indicating potential improvements in the system's reliability over time. The acceptable range of failure rate would depend on the specific requirements and objectives of the project. It's essential to ensure that the observed failure rate aligns with project specifications and reliability targets.

Furthermore, it's crucial to monitor the trend of the failure rate over time. A decreasing trend suggests positive reliability growth, while a stable or increasing trend may indicate underlying issues that require attention.

In conclusion, while there isn't a universally applicable range for failure rate, it's essential to consider project-specific requirements and objectives when determining the acceptable range of failure rate for the test data. Monitoring the trend of the failure rate over time is also important for assessing reliability growth and making informed decisions regarding system improvements and modifications.

# Assessment Using Reliability Demonstration Chart

#

# Comparison of Results

# Discussion on Similarity and Differences of the Two Techniques

# How the team work/effort was divided and managed

#

# Difficulties encountered, challenges overcome, and lessons learned

# Comments/feedback on the lab itself
