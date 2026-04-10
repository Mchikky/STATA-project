# STATA Project

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

### Recommendations
- Since teaching methods have a significant impact on student performance, further analysis should be conducted to identify which specific methods differ.
- The most effective teaching method, lecture (i.e., the one associated with the highest mean score of 81.5) should be prioritized for wider adoption.
- Due to the significantly lower scores, in workshop, 46.5, teacher training programs should be implemented to improve their effectiveness or phase them out in favor of better-performing methods.
- Additional factors (such as teacher experience, student engagement, or classroom resources) should be considered in future studies to improve teaching strategies.
<img width="4493" height="427" alt="image" src="https://github.com/user-attachments/assets/5d8d7830-265a-4daa-9878-98469b8e65fe" />




   
   
## Question Two: Study the dataset on the Second National Health and Nutrition Examination Survey using “webuse nhanes2l” 
Import dataset and clean 
#### <img width="839" height="506" alt="image" src="https://github.com/user-attachments/assets/bbb4bdb2-a778-4a2b-8593-026f0c5d4e4c" />
browse to show dataset
#### <img width="1182" height="232" alt="Captureq" src="https://github.com/user-attachments/assets/61042951-f83e-49ad-9e6c-4121b1a81d2f" />
#### <img width="720" height="345" alt="CaptureSu" src="https://github.com/user-attachments/assets/b407847e-cc96-45d1-ac27-c4d0cf657cf8" />
#### <img width="788" height="348" alt="CaptureDe" src="https://github.com/user-attachments/assets/04ae8300-d003-4f39-be28-42d7a7502f1c" />
#### <img width="419" height="165" alt="Captureq1" src="https://github.com/user-attachments/assets/c332507c-3749-40b1-aedd-806fbef030e3" />
#### <img width="432" height="218" alt="Captureq2" src="https://github.com/user-attachments/assets/da10fa49-20c7-4863-86df-e8d67dea3c3a" />

### a.	Run the simple regression analysis using the appropriate variables, state the rationale behind your decision
Check conditions for regression: linearity of relationships between the dependent and independent variables, normality of residues, homoscedasticity of the residues, no influencial points (outliers), independence of the observations
#### <img width="569" height="489" alt="CaptureAs" src="https://github.com/user-attachments/assets/8534c93b-65d3-41ae-9cc5-f947619bc803" />
histogram age
#### <img width="679" height="472" alt="CaptureAge" src="https://github.com/user-attachments/assets/7db54472-8ebc-4bf2-a7c1-9d7aebb89f21" />
histogram bmi
#### <img width="681" height="479" alt="CaptureBMI" src="https://github.com/user-attachments/assets/96eadbeb-5aa8-47d1-b857-5b425842c95b" />
sktest
#### <img width="634" height="305" alt="Capturesk" src="https://github.com/user-attachments/assets/9e856d48-665e-427a-822f-ad0bd6808bab" />
qnorm bmi
#### <img width="681" height="475" alt="Capturebm" src="https://github.com/user-attachments/assets/b61824ba-f26d-4326-8b24-aa8f85c1d6cd" />
qnorm age
#### <img width="685" height="481" alt="CaptureAg" src="https://github.com/user-attachments/assets/91816208-a887-47e7-937e-e365c0e406e4" />
No perfect multicolinearity
#### <img width="773" height="465" alt="CaptureVIF" src="https://github.com/user-attachments/assets/f0b7e08c-0243-417d-b310-a14aed15aef8" />
Homoscedasticity
#### <img width="737" height="496" alt="CapturerRV" src="https://github.com/user-attachments/assets/afaeef3f-f3eb-4be6-bf2e-59c9b74743cc" />
Simple regression
#### <img width="576" height="143" alt="CaptureRe" src="https://github.com/user-attachments/assets/7da6b861-ebb2-4be8-acc2-18724af9968c" />
#### <img width="595" height="276" alt="CaptureREg" src="https://github.com/user-attachments/assets/c3210b52-433d-4aeb-a18f-3000d2cebf39" />

### b.	Run multiple regression analysis on the relevant variables and also interpret your findings with justification
Multiple regression
#### <img width="430" height="37" alt="CaptureM" src="https://github.com/user-attachments/assets/e174e085-b99c-4d2b-a5ba-22665e36b87e" />
#### <img width="690" height="315" alt="CaptureMR" src="https://github.com/user-attachments/assets/b559b7ce-d758-4d6e-a617-88174f5f21a4" />

### c.	Perform logistic regression on the relevant dependent and independent variables and state your reason for the selection of the variables
Logistic regression 
#### <img width="872" height="109" alt="CaptureLog" src="https://github.com/user-attachments/assets/02f6593f-6a87-4929-9463-04d5865d53e5" />
#### <img width="693" height="302" alt="CaptureLo" src="https://github.com/user-attachments/assets/0526a41d-df66-42a9-b724-6200c5a4afdf" />
 
### d.	Run ttest on some of the relevant variables and also interpret your findings
t-test determines if there is statistically significant different between the means of 2 groups
#### <img width="994" height="142" alt="CaptureTT" src="https://github.com/user-attachments/assets/9cafd301-845e-4271-9015-3335b7438ab3" />
#### <img width="693" height="339" alt="Capturetet" src="https://github.com/user-attachments/assets/8d10bd16-6a94-4f8a-bae9-51f97d5240b0" />

### e.	Observe the relevant variables and run analysis of variance (ANOVA)
anova compares the means among 3 or more groups
#### <img width="776" height="298" alt="CaptureAno" src="https://github.com/user-attachments/assets/e8700617-1548-4365-86f4-50325157824c" />
#### <img width="843" height="72" alt="CaptureAN" src="https://github.com/user-attachments/assets/ffe619c3-d87b-4540-8870-34d794ed2540" />
#### <img width="692" height="276" alt="CaptureAnov" src="https://github.com/user-attachments/assets/d65f3b84-cbf4-4e36-b830-e9d97215ff13" />
###

Age-based screening programs should be reinforced, especially for older individuals. Although BMI was not significant in this analysis, weight management should still be encouraged as part of a healthy lifestyle. 
Public health campaigns should emphasize the importance of weight management to control MAP and reduce the risk of cardiovascular diseases. 
Routine screening for Mean Arterial Pressure (MAP) in high-risk groups targeting individuals with elevated MAP levels, as they are strongly associated with hypertension.
While race shows statistical significance, its low explanatory power suggests that other factors (e.g., diet, lifestyle, genetics) might play a larger role in determining MAP. 
<img width="4368" height="329" alt="image" src="https://github.com/user-attachments/assets/5ddd2999-7839-4fde-a0e2-4d50d8ef1036" />


