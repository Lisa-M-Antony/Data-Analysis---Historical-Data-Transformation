As a part of the Data Analyst Intern assignment - exercise 1 I was given with a csv file 'input', containing employee data. The data given was in columnar format which I am asked to transform into a historical, row-based versioning format suitable for database storage using Python.
The given data consisted the columns 'Employee Code', 'Manager Employee Code, 'Compensation', 'Compensation 1', 'Compensation 1 Date', ' Compensation 2', 'Compensation 2 Date', 'Review 1', 'Review 1 Date', 'Review 2', 'Review 2 Date', 'Engagement 1', 'Engagement 1 Date', 'Engagement 2', and 'Engagement 2 Date'.
I have loaded the necessary libraries in the Jupyter notebook. 
The next step was to load the 'input' csv file into a Pandas DataFrame. 
After defining the transform_data function, I have extracted the employee information, compensation data, review data, and engagement data to convert them into a historical format. 
I have determined the effective dates and end dates for each record in a way that the column 'Effective Date' contains all the dates on which there's an occurrence in the input data and the column 'End Date' consists of the date that's one day before the effective date in the next row. I have assigned a far-future date 2100-01-01 for the latest record of an employee.
Created rows for each period with consistent data. 
Additionally, I have defined a function to get dates in between two dates. 
Then I calculated the End Date and added the columns to the output file. 
Transformed the data to a DataFrame. 
Saved the transformed data into a new csv file which contains the columns 'Employee Code', 'Manager Employee Code', 'Last Compensation', 'Compensation', 'Last Pay Raise Date', 'Variable Pay', 'Tenure in Org', 'Performance Rating', 'Engagement Score', 'Effective Date' and 'End Date'. 
Finally, I have displayed the transformed data.
