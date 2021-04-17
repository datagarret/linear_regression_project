# Linear Regression Project #

## Analysis Outline: Final Project ##

### Research Question ###
The research question is a part of an exploratory observational study exploring the relationship between infection surveillance, control programs and the reduction of hospital-acquired infection rates. Does the average length of stay in the hospital affect the infection risk of nosocomial infections?

-	Primary outcome: infection risk, the average estimated probability of acquiring infection in the hospital (percent)

-	Main exposure: length of stay, the average length of stay of all patients in hospitals

### Data set description ###
The SENIC Project, the Study on the Efficacy of Nosocomial Infection Control, was a random sample of 113 hospitals among 338 hospitals originally surveyed. The study period was from 1975-1976. The primary objective was to determine if infection surveillance and control programs reduce the rates of hospital-ac quired infection in the United States.

### Variables ###

  - Identification number: ordinal data, used to identify observation and provides information for other variables for a single hospital 
  - Length of stay: the average length of stay of all patients in hospitals (day)s (Quantitative, continuous)
  - Age: verage age of the patients (years) (quantitative, continuous)
  - Infection risk: the average estimated probability of acquiring infection in the hospital (percent) (Quantitative, continuous)
  - Routine culturing ratio: ratio of the number of cultures performed to number of patients without signs or symptoms of hospital-acquired infection, times 100 (quantitative, continuous)
  - Routine chest X-ray ratio: ratio of the number of X-rays performed to number of patients without signs or symptoms of pneumonia, times 100 (quantitative, continuous)
  - Number of beds: average number of beds in the hospital during the study period (Quantitative, continuous)
  - Medical school affiliation: 1=yes, 2=no
  - Region: geographic region, 1=NE, 2=NC, 3=S, 4=W
  - Average daily census: average number of patients in the hospital per day during the study period (quantitative, continuous)
  - Number of nurses: average number of full-time equivalent and licensed practical nurses during the study period (number of full-time + 1.5 the number of part-time nurses)
  - Available facilities and services: percent of 35 potential facilities and services that are provided by the hospital


 
### Analysis strategy ###
  1.	Look at the data
  2.	Fit the preliminary model 
  3.	Perform diagnostics
    a.	Residuals from preliminary model; assess normality (proc univariate, box-plot, Shapiro- Wilk test, ANOVA), constant variance (scatter plot matrix vs each         predictor, Breuscho-pagan test), and linearity (Q-Q plot)
    b.	Check of outliers using semistudentized residuals 
  4.	Fix problems
     a.	Explore interaction, box-cox transformation, outliers, consider categorizing variables such as complications: 1 if yes; 0 if no, using no as the reference. The same consideration for drugs, instead of considering the number of drugs tracked, I propose to reform the variable as “does the individual have tracked drugs prescribed?” 1 if yes; 0 if no. Explore Higher order terms 
     b.	Use methods of variable selection 
        i.	Explore missingness 
        ii.	Confounding 
        iii.	Model selection and validation strategies from chapter 9 will be employed as relevant 
     c.	Compare models using likelihood ratio tests for which model is best fit for the data, inference, ANOVA F, mean prediction 
  5.	Fit new model 
  6.	Diagnose new model
    a.	Influential point analysis strategies from chapter 10 will be employed as relevant.
  7.	Repeat steps 4-6 until all assumptions are met
  8.	Final inference 

