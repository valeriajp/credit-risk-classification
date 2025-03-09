# Credit-Risk-Classification
![20943799](https://github.com/user-attachments/assets/0abf1c92-d0dd-4711-9de3-568c486b10d3)

# Background
In this Challenge, you’ll use various techniques to train and evaluate a model based on loan risk. You’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

# Before You Begin
1. Create a new repository for this project called ![image](https://github.com/user-attachments/assets/be89d174-5b3a-4098-ad2c-89e8dff9bf94). **Do not add this homework to an existing repository.**
2. Clone the new repository to your computer.
3. Inside your ![image](https://github.com/user-attachments/assets/4261223b-9092-4c14-85d9-2ceecb17bec4) repository, create a folder titled "Credit_Risk."
4. Inside the "Credit_Risk" folder, add the ![image](https://github.com/user-attachments/assets/4b5adfb3-e005-4e14-b5c1-291c19e2cc51) and ![image](https://github.com/user-attachments/assets/9d7b75a1-e3d7-4fa1-a526-6b7f988c04dc) files found in the "Starter_Code.zip" file.
5. Push your changes to GitHub.

# Instructions
The instructions for this Challenge are divided into the following subsections:
- Split the Data into Training and Testing Sets
- Create a Logistic Regression Model with the Original Data
- Write a Credit Risk Analysis Report (included in files attached) 

# Split the Data into Training and Testing Sets
Open the starter code notebook and use it to complete the following steps:
1. Read the ![image](https://github.com/user-attachments/assets/f6ba785b-8303-4120-8d71-75e5e825372f) data from the Resources folder into a Pandas DataFrame.
2. Create the labels set (![image](https://github.com/user-attachments/assets/c386faf0-e16e-4718-bcd6-11453af09b2e)) from the “loan_status” column, and then create the features (![image](https://github.com/user-attachments/assets/dfbc60cc-ecba-43eb-80b7-1bb52fe94b57)) DataFrame from the remaining columns.

> **📌 NOTE**  
> A value of 0 in the `"loan_status"` column means that the loan is healthy.  
> A value of 1 means that the loan has a high risk of defaulting.

3. Split the data into training and testing datasets by using ![image](https://github.com/user-attachments/assets/7e2c26ac-bb0c-473d-956c-8b1989224f70).

# Create a Logistic Regression Model with the Original Data
Use your knowledge of logistic regression to complete the following steps:
1. Fit a logistic regression model by using the training data (![image](https://github.com/user-attachments/assets/bc3f9654-6eb4-4012-9473-75de9cd01b71) and ![image](https://github.com/user-attachments/assets/2ee1f1c3-57d9-4890-8eca-73638624aead)).
2. Save the predictions for the testing data labels by using the testing feature data (![image](https://github.com/user-attachments/assets/398cfbb6-3b49-4929-8f86-c0d527236540)) and the fitted model.
3. Evaluate the model’s performance by doing the following:
   - Generate a confusion matrix.
   - Print the classification report.
4. Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

# Write a Credit Risk Analysis Report
Write a brief report that includes a summary and analysis of the performance of the machine learning models that you used in this homework. You should write this report as the ![image](https://github.com/user-attachments/assets/c7392cf4-73a0-407b-8813-66746b8f7b17) file included in your GitHub repository.
Structure your report by using the report template that ![image](https://github.com/user-attachments/assets/2285257b-4903-4cff-acad-030c348c7afa) includes, ensuring that it contains the following:
1. *An overview of the analysis:* Explain the purpose of this analysis.
2. *The results:* Using a bulleted list, describe the accuracy score, the precision score, and recall score of the machine learning model.
3. *A summary:* Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning.

# Requirements
# Split the Data into Training and Testing Sets (30 points)
To receive all points, you must:
- Read the ![image](https://github.com/user-attachments/assets/01e0b198-06a6-46e3-9445-8ddc70ec724a) data from the Resources folder into a Pandas DataFrame. (5 points)
- Create the labels set (![image](https://github.com/user-attachments/assets/c386faf0-e16e-4718-bcd6-11453af09b2e)) from the “loan_status” column, and then create the features (![image](https://github.com/user-attachments/assets/dfbc60cc-ecba-43eb-80b7-1bb52fe94b57)) DataFrame from the remaining columns. (10 points)
- Split the data into training and testing datasets by using ![image](https://github.com/user-attachments/assets/94a091fd-5421-4931-a453-4f2e73e05ea6). (15 points)

# Create a Logistic Regression Model (30 points)
To receive all points, you must:
- Fit a logistic regression model by using the training data (![image](https://github.com/user-attachments/assets/b5bbdda7-7402-4ab9-abfb-4b22f2f1098e)and ![image](https://github.com/user-attachments/assets/e983f5ee-4dbc-48b2-873f-3fdfc6ffb84a)). (10 points)
- Save the predictions on the testing data labels by using the testing feature data (![image](https://github.com/user-attachments/assets/cdd612bd-7d42-42bf-ba1d-724f6c2c37ad)) and the fitted model. (5 points)
- Evaluate the model’s performance by doing the following:
  - Generate a confusion matrix. (5 points)
  - Generate a classification report. (5 points)
  - Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels? (5 points)

# Write a Credit Risk Analysis Report (20 points)
To receive all points, you must:
- Provide an overview that explains the purpose of this analysis. (5 points)
- Using a bulleted list, describe the accuracy, precision, and recall scores of the machine learning model. (5 points)
- Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning. (10 points)

# Coding Conventions and Formatting (10 points)
To receive all points, you must: 
- Place imports at the top of the file, just after any module comments and docstrings and before module globals and constants. (3 points)
- Name functions and variables with lowercase characters, with words separated by underscores. (2 points)
- Follow DRY (Don’t Repeat Yourself) principles, creating maintainable and reusable code. (3 points)
- Use concise logic and creative engineering where possible. (2 points)

# Code Comments (10 points)
To receive all points, your code must:
- Be well commented with concise, relevant notes that other developers can understand. (10 points)

# References
Data for this dataset was generated by edX Boot Camps LLC, and is intended for educational purposes only.
