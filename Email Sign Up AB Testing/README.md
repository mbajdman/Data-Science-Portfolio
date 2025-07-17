A/B Testing with Python

File: AB Testing Email Sign-Up.ipynb

Overview: 

Evaluated the impact of changing the colour of the sign-up button. Compared the sign-up rates for the original & new button & determined if this seemingly minor design change could lead to a significant improvement in user conversions.

Key Features:

Data Exploration and Analysis: Analysing pre-test and test data, including daily visitor counts and sign-up rates.
Hypothesis Formulation: Defining the null and alternative hypotheses for the A/B test.
Experiment Design: Determining key parameters such as significance level (alpha), statistical power, minimum detectable effect (MDE), and calculating the required sample size and experiment duration.
Validity Threat Assessment: Performing an AA test to ensure group comparability and a Sample Ratio Mismatch (SRM) check using the Chi-Square test to validate the randomisation algorithm.
Statistical Inference: Applying Chi-Squared and T-Tests for proportions to compare the sign-up rates of the control and treatment groups.
Confidence Interval Analysis: Calculating and interpreting confidence intervals for the difference in sign-up rates to understand the range of potential improvement.
Launch Decision: Making a data-driven recommendation based on the statistical significance and practical impact of the experiment results.

Technologies:

Python,
Pandas,
SciPy,
statsmodels,
seaborn

Expected Outcomes:

Determination of the impact of button colour on sign-up rates: A clear conclusion on whether changing the sign-up button colour from blue to green has a statistically significant impact on the sign-up rate.
Quantification of the lift (if any) in sign-up rate: A measurement of the percentage increase or decrease in sign-up rate observed in the treatment group compared to the control group.
Assessment of the experiment's validity: Confirmation that the experiment design and execution were sound, based on the AA test and SRM check results.
Recommendation for future action: A data-backed decision on whether to implement the green button or maintain the original blue button.
Insights into user behaviour: Potential insights into how a seemingly small design change can influence user conversion.
