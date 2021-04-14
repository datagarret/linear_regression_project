# Linear Regression Project

Analysis Outline: Final Project

•	Research Question: The research question is a part of an exploratory observational study exploring the relationship between total cost of insurance claims by a subscriber and the number of comorbidities. Does the number of comorbidities affect the total cost of claims made by a subscriber?
o	Primary outcome: total cost of claims by subscriber (dollars)
o	Main exposure: number of other diseases that the subscriber had during the period
•	Data set description: The data set was collected information from 788 individuals from an insurance company who made claims resulting from ischemic (coronary) heart disease. Information was collected on total costs and 9 variables were collected based on the possibilities of influencing the total cost of insurance claims. Data was collected from January 1, 1998 through December 31, 1999. 
o	Variables:
	Identification number: ordinal data, used to identify observation and provides information for other variables 
	Total cost: total cost of claims by subscriber (dollars)
•	Quantitative, continuous 
	Age: age of the subscriber (years)
•	 Quantitative, continuous
	Gender: gender of subscriber (1 if male; 0 otherwise)
•	categorical, dichotomous 
	Interventions: total number of interventions or procedures carried out
•	 Quantitative, continuous
	Emergency room visits: number of emergency room visits
•	Quantitative, continuous
	Complications: number of other complications that arose during heart disease treatment 
•	 Quantitative, continuous
	Comorbidities: number of other diseases that the subscriber had during the period 
•	Quantitative, continuous
	Duration: number of days of duration of treatment condition
•	 Quantitative, continuous
•	Analysis strategy 
1.	Look at the data
2.	Fit the preliminary model 
3.	Perform diagnostics
a.	Residuals from preliminary model; assess normality (proc univariate, box-plot, Shapiro- Wilk test, ANOVA), constant variance (scatter plot matrix vs each predictor, Breuscho-pagan test), and linearity (Q-Q plot)
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

