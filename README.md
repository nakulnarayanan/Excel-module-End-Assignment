# Excel-module-End-Assignment
Excel module End Assignment
**Data Cleaning:  (5 marks) **
1) Check for the number of missing values marked with '?' in each column of the “Medical 
Examinations” Table and "Hospitalization Details" Table.  2 ? In smoker column	6 ? In customer id	3 in month, 1 in city tier,1 in hospital tier, 2 in state
2) Fill in the missing values of ‘month’ with Sep and ‘year’ with its average rounded to the 
nearest integer.  Done
3) Determine the most frequently occurring values in the ‘smoker’, 'Hospital tier' and 'City 
tier' columns, and fill in the missing values accordingly.  - Filled with mode
4) If any 'State ID' values are missing, consider filling them with 'Unknown' or using another 
appropriate strategy. - Filled with mode

**Data Transformation:  (8 marks) **
1) Split the ‘names’ column in the “Customer Names” Table into 3 meaningful columns: 
‘Title’, ‘First Name’, and ‘Last Name’. Done
2) Convert the "NumberOfMajorSurgeries" column in the “Medical Examinations” Table to 
numerical data by replacing non-numeric characters with meaningful numerical values.  Added as 0
3) Check for inconsistencies in the 'Heart Issues' and 'smoker' columns and propose 
corrective actions if necessary.  Corrected yes to Yes using capitalize each word option
4) Create a new column named “Weight Status” that categorizes BMI into different 
categories as below:  =IFS([@BMI]>=30,"Obesity",[@BMI]>=25,"Overweight",[@BMI]>=18.5,"Normal Weight",TRUE,"Underweight")
5) Create a new column named “Diabetes Status” and fill it as per the information given 
below: =IFS([@HBA1C]<5.7,"Normal",[@HBA1C]<=6.49,"Pre Diabetes",[@HBA1C]>=6.5,"Diabetes")
6) Merge ‘year’, ‘month’ and ‘date’ columns in the “Hospitalization Details” Table into one 
column named ‘Date of Birth’ and format it in ‘DD-MMM-YYYY’ custom format.  used &. then used =datevalue() function.
7) Calculate the ‘Age’ of each customer based on their ‘Date of Birth’ and the date of 
collection of the dataset, which is 8thJune 2023. -=DATEDIF([@DOB],"08-06-2023","Y")
8) Format ‘charges’ column as currency ($). Done
