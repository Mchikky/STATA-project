# Capstone Project

## Question One: 
The table below describe the test score for three students using three techniques such as lecture, workshop and online learning, kindly use the appropriate test statistic to test significant mean difference in the score using the three-teaching method at 5% level of significant
### <img width="632" height="142" alt="Capture1" src="https://github.com/user-attachments/assets/40436b96-2136-4015-91c0-43bfd0a88686" />
#### State the command to be used in entering the information into Stata window. 
Write the commands in the Stata dofile and keep log of the output
#### <img width="556" height="432" alt="Capture2" src="https://github.com/user-attachments/assets/a31b9cac-8d7f-43e6-9bfd-5e8073061672" />
#### <img width="199" height="273" alt="CaptureA" src="https://github.com/user-attachments/assets/b7a214f1-551a-4ee2-a1ec-b7d0265201cc" />
#### <img width="518" height="127" alt="CaptureAA" src="https://github.com/user-attachments/assets/67c94ec7-7a79-453c-bfeb-b2bb6be2ce44" />
#### <img width="617" height="204" alt="CaptureAAA" src="https://github.com/user-attachments/assets/a3c83c1f-1c2e-4351-9a95-44eb1b3e5d9d" />
#### <img width="417" height="176" alt="CaptureAAAA" src="https://github.com/user-attachments/assets/c7281913-32eb-4997-84cf-687cce3204d5" />
#### <img width="464" height="132" alt="CaptureAAAAA" src="https://github.com/user-attachments/assets/3bdc28fe-118f-4328-8b34-2566cc8e4333" />

#### a.	What is the dependent variable? and state the reason for your response
 The dependent variable is the Test scores. Reason: The test score is the outcome that depends on the teaching method used.

#### b.	What is the independent variable? Give reason for your response
 The independent variable is the Teaching methods which are Lecture, Workshop and Online learning. Reason is teaching methods affect students performance.

#### c.	What type of statistical technique is appropriate for the analysis? State reason for your response
The statistical technique appropriate for the analysis is One way analysis of variance (ANOVA). Reason: There is one dependent variable and 3 independent variables. So we are considering the mean of one dependent variable and 3 independent variables

#### d.	What type of statistics is the test used, and why is it so? The type of statistics test used is Inferential Statistics. Reason: The test used in this case is inferential statistics because we are making conclusions about the population based on sample data. Specifically, we use One-Way ANOVA (Analysis of Variance) to determine if there is a statistically significant difference in mean test scores among the three teaching methods. 

#### e.	What type test does the technique belongs to?
The test type belongs to Parametric Test. Reason: ANOVA is a parametric test as it assumes normality and homogeneity of variance in the data

#### f.	What is the Stata command for the analysis?
#### <img width="308" height="95" alt="CaptureA6" src="https://github.com/user-attachments/assets/930feaec-3ab8-45d7-8c91-1e318070798e" />
Histogram
#### <img width="677" height="484" alt="Capturef2" src="https://github.com/user-attachments/assets/bf7a98d9-1ebe-4bb5-accb-9e97061c2c12" />
Q-Q plot, qnorm: quantile function of normal distribution
#### <img width="674" height="489" alt="Capturef3" src="https://github.com/user-attachments/assets/74d459d5-910c-4bb9-89db-d4313718dc67" />
anova score teaching_method
#### <img width="622" height="266" alt="Capturef4" src="https://github.com/user-attachments/assets/fb185ea7-cf9e-4d9b-b318-9208cca34f5c" />

#### g.	Interpret your findings
   Ho= There is no significant difference in the mean score among the three teaching methods
   Ha= At least one teaching methods has a significantly different mean score
   From our ANOVA result F-value 28.75  P-value is 0.0001 &  R squared value is 0.8646.
   Since the P-value is 0.001(<0.05), we do not have enough evidence to support the null hypothesis
   This means there is a statistically significant difference in mean scores between at least one of the teaching methods.
   Since the R-squared is 0.8646, it means 86.46% of the variation in test scores is explained by the teaching method
   
   
## Question Two: Study the dataset on the Second National Health and Nutrition Examination Survey using “webuse nhanes2l” 
Import dataset and clean 
#### <img width="839" height="506" alt="image" src="https://github.com/user-attachments/assets/bbb4bdb2-a778-4a2b-8593-026f0c5d4e4c" />
#### <img width="720" height="345" alt="CaptureSu" src="https://github.com/user-attachments/assets/b407847e-cc96-45d1-ac27-c4d0cf657cf8" />
#### <img width="788" height="348" alt="CaptureDe" src="https://github.com/user-attachments/assets/04ae8300-d003-4f39-be28-42d7a7502f1c" />
#### <img width="419" height="165" alt="Captureq1" src="https://github.com/user-attachments/assets/c332507c-3749-40b1-aedd-806fbef030e3" />
#### <img width="432" height="218" alt="Captureq2" src="https://github.com/user-attachments/assets/da10fa49-20c7-4863-86df-e8d67dea3c3a" />

### a.	Run the simple regression analysis using the appropriate variables, state the rationale behind your decision


### b.	Run multiple regression analysis on the relevant variables and also interpret your findings with justification
Check conditions for multiple regression: linearity of relationships between the dependent and independent variables, normality of residues, homoscedasticity of the residues, no influencial points (outliers), independence of the observations

### c.	Perform logistic regression on the relevant dependent and independent variables and state your reason for the selection of the variables
### d.	Run ttest on some of the relevant variables and also interpret your findings
### e.	Observe the relevant variables and run analysis of variance (ANOVA)
