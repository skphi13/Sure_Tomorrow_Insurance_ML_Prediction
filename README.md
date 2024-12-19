# Sure_Tomorrow_Insurance_ML_Prediction
The Sure Tomorrow company needs a machine learning model that can predict whether or not a customer is likely to receive an insurance benefit.

- Task 1: Find customers who are similar to a given customer. This will help the company's agents with marketing.
- Task 2: Predict whether a new customer is likely to receive an insurance benefit. Can a trained prediction model do better than an untrained dummy model? Can it do worse? Explain your logic.
- Task 3: Predict the number of insurance benefits a new customer is likely to receive using a linear regression model.
- Task 4: Protect clients' personal data without breaking the model from the previous task.


## Data Description

`/datasets/insurance_us.csv`
- Features: insured person's gender, age, salary, and number of family members.
- Target: number of insurance benefits received by an insured person over the last five years.

## Conclusion:

- Implemented K-Nearest Neighbors (KNN) to identify customers similar to a given customer, enhancing predictions through data scaling and the use of the Euclidean distance metric.

- Developed models for the marketing team to predict the likelihood of customers receiving insurance benefits. The final model, using scaled data, achieved a high F1 score of 92% on the validation set, significantly outperforming a dummy model.

- Constructed a Linear Regression model to predict the number of insurance benefits a new customer may receive, yielding a moderately high R² score of 66%. It was noted that scaling the data did not notably affect the results.

- Applied data obfuscation techniques, demonstrating analytically that the obfuscated data produced no significant differences compared to the original data.

- Conducted computational tests by training a Linear Regression model on the obfuscated data, confirming that the resulting RMSE and R² scores matched those obtained with the original data, thereby validating the effectiveness of the obfuscation process.
