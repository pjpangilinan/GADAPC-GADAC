# GADAPC-GADAC: Predicting Employee Turnover with Logistic Regression and KNN Models in Salifort Motors

see [Project Proposal](https://github.com/pjpangilinan/GADAPC-GADAC/blob/main/GADAC-Act.pdf) <br>
see [Jupyter Notebook](https://github.com/pjpangilinan/GADAPC-GADAC/blob/main/GADAC-C7.ipynb) <br>


## Plan Phase

### Who are your stakeholders for this project?
* Salifort Motors’ HR department, 
* Senior leadership and management teams, 
* Current employees 
### What are you trying to solve or accomplish? 
* Predict which employees are likely to leave
* Identify key factors influencing employee turnover 
* Provide recommendations to improve employee retention and satisfaction
### What are your initial observations when you explore the data? 
* There are numerical variables (e.g., satisfaction_level, average_monthly_hours) and categorical variables (e.g., Department, salary) 
* Variables like promotion, work accident, and department might have significant influence on turnover
### What resources do you find yourself using as you complete this stage? (Make sure to include the links.)
* [HR Dataset from Kaggle](https://www.kaggle.com/datasets/mfaisalqureshi/hr-analytics-and-job-prediction?select=HR_comma_sep.csv)
* [Pandas Documentation](https://pandas.pydata.org/docs/)
### Do you have any ethical considerations in this stage? 
* Handle private employee data with care
* Avoid biased modeling that could unfairly target certain groups or departments

## Analyze Phase

### What did you observe about the relationships between variables?
* Based on the correlation heatmap, employee satisfaction has the strongest negative relationship with turnover, meaning less satisfied employees are more likely to leave. Longer tenure is also linked to higher retention, while factors like last evaluation, number of projects, and average monthly hours show little direct connection to leaving. Work accidents slightly reduce the chance of leaving, and recent promotions have minimal impact. Overall, satisfaction and tenure stand out as the key indicators of employee departure.
### What do you observe about the distributions in the data?
* The satisfaction level and last evaluation scores are mostly skewed towards higher values, but employees who left tend to have a wider range of satisfaction scores. The number of projects and monthly hours are somewhat spread out but show clusters where employees working very long hours or on many projects are more likely to leave. The salary distribution is imbalanced, with most employees in the lower and medium salary groups.
### What transformations did you make with your data? Why did you chose to make those decisions?
* Since there were categorical variables in the dataset, one-hot encoding was used to allow for machine learning. The numerical variables were scaled using the MinMaxScaler. These decisions were made to ensure the models can interpret and learn from the data effectively.
### What are some purposes of EDA before constructing a predictive model?

### What resources do you find yourself using as you complete this stage? (Make sure to include the links.)
* [pandas Documentation](https://pandas.pydata.org/docs/)
* [matplotlib Documentation](https://matplotlib.org/stable/users/index.html)
* [seaborn Documentation](https://seaborn.pydata.org/)
### Do you have any ethical considerations in this stage?
* The ethical considerations in this stage is the same as the first.

## Construct Phase

### Which independent variables did you choose for the model and why?
* I chose every parameter except for the "left" parameter since that is the dependent variable. Satisfaction and tenure showed stronger correlations, while the others may still provide useful context.
### How well does your model fit the data?
* The model achieves good accuracy (around 83%-95% depending on the method) and balanced precision and recall, suggesting it fits the data well for predicting employee turnover.
### Can you improve it? Is there anything you would change about the model?
* To improve the model, I might try feature engineering (combining or transforming variables) and try other algorithms like Random Forest or XGBoost,
### What resources do you find yourself using as you complete this stage? (Make sure to include the links.)
* [scikit-learn Documentation](https://scikit-learn.org/stable/)
### Do you have any ethical considerations in this stage?
* The ethical considerations in this stage is the same as the those before.

## Execute Phase

### What key insights emerged from your model(s)?
* The models revealed that employee satisfaction, tenure, number of projects, and average monthly hours are significant predictors of whether an employee leaves. Employees with low satisfaction, longer time without a promotion, and high workloads are more likely to leave.
### What business recommendations do you propose based on the models built?
* To reduce turnover, the company should focus on improving employee satisfaction through better work-life balance, capping the number of projects assigned, and offering timely promotions or career development opportunities.
### What potential recommendations would you make to your manager/company?
* Make sure to regularly survey your employees to ensure that their satisfied with their job (workload/position). Also, have clear policies to promote tenured staff to keep them.
### Do you think your model could be improved? Why or why not? How?
Since the hyperparameters were already tuned, I believe that the model could be further improved by adding more parameters that could have a significant impact on employees leaving.
### Given what you know about the data and the models you were using, what other questions could you address for the team?
* What factors contribute most to employee satisfaction?
* How do specific departments or roles influence turnover rates?
### What resources do you find yourself using as you complete this stage? (Make sure to include the links.)
* [scikit-learn Documentation](https://scikit-learn.org/stable/)
* [pandas Documentation](https://pandas.pydata.org/docs/)
* [matplotlib Documentation](https://matplotlib.org/stable/users/index.html)
* [seaborn Documentation](https://seaborn.pydata.org/)
### Do you have any ethical considerations in this stage?
* The ethical considerations in this stage is the same as the those before.

