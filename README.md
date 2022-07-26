# MCD4710
MCD4710 - Introduction to Algorithms and Programming

Task 1: Read the data into a table

Implement a function named read_data(filename), with the following specification, which reads a given file and returns the contents in a table. Make sure you store the smoking status (in the 6th column) as an integer and the other numerical values as floats.

Task 2: Convert the weight to kilograms

The weight of each patient is given in pounds (lbs). Write a function named lbs_to_kg(table), which converts the weight to kilograms (kg) and replaces the original weight in the table, for each patient. Make sure the weight in kg is rounded to one decimal place.

def lbs_to_kg(table):
  
Task 3: Calculate the body mass index (BMI)

The body mass index (BMI) for each patient needs to be calculated. Write a function named calculate_BMI(table), which calculates the BMI for each person, using the formula below. Append the BMI values, rounded to one decimal place, as the last column of the table.

Task 4: Categorize based on BMI

The patients in the data table need to be categorized according to their BMI value. Write a function named categorise(table) that determines the category for each person based on the following classification and store characters U, N or O for underweight, normal and obese, respectively. This information should be stored next to their BMI value in the table. The categorization should be done according to the following classification.

Task 5: Look up BMI value of a given patient

Write a function named get_BMI(table,name) that returns the BMI value of a given patient by looking up the name in the table. If the given name is not available in the table, the function should return None. You may assume that the names are unique.

Task 6: Look up blood pressure value of a given patient

Write a function named get_BP(table,name) that returns the blood pressure readings as a tuple, (systolic, diastolic), of a given patient by looking it up in the table. Make sure the blood pressure readings are returned as integer values. If the given name is not available in the table, the function should return None. You may assume that the names are unique.

Task 7: Determine whether a given patient is a smoker or not

Write a function named is_smoker(table,name) that returns True if the given patient is a smoker and False if not. The function should return None if the patient record is not available in the table.

def is_smoker(table,name):
  data = table[table.iloc[:,0] == name]
  if data[5] == 1:
    return True
  return False

Task 8: Extract the records of high-risk patients and write to a separate csv file

Now we need to extract the records of high-risk patients from the table and save their details (all column values of the patient in the table) into a new csv file. Write a function named extract_high_risk(table,filename) that extracts the records of patients who satisfy all of the following conditions and write their data into the given file, output_filename. Add the column headings to the file as well.

有需求请联系
