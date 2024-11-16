# Python for Data Science - Assignments

## Introduction
This repository contains assignments completed as part of the Python for Data Science course. The goal of this course is to develop proficiency in using Python for various data analysis and manipulation tasks, covering foundational programming concepts, data structures, and basic data processing techniques. Each assignment demonstrates practical applications of Python, with detailed explanations provided for clarity.

## Topics Covered
- Basic Python syntax and operations
- Variables and data types
- Conditional statements and loops
- Functions and error handling
- Lists, dictionaries, and other data structures
- File handling and data manipulation
- Libraries for data science (NumPy, Pandas, etc.)
- Object-oriented programming
- Data visualization

Each section describes the assignment and its objectives, followed by an explanation of the solution implemented.

---

## Assignment 1: Introduction to Python

### Objective
The first assignment focuses on building familiarity with basic Python syntax and foundational programming constructs. Key concepts such as printing messages, performing arithmetic operations, and working with variables, lists, and dictionaries are introduced.

### Tasks and Solutions
1. **Print a greeting message**  
   This task involves printing a simple greeting message using Python's `print()` function.
   
2. **Arithmetic operations**  
   Students are required to perform basic arithmetic operations such as addition, subtraction, multiplication, and division using predefined variables.

3. **Personalized greeting**  
   This task demonstrates how to define a variable and use it in a formatted string to print a personalized message.

4. **List operations**  
   Create and manipulate a list containing several elements (e.g., university names) and demonstrate list indexing.

5. **Dictionary operations**  
   Create a dictionary with student information and iterate through its key-value pairs to display them.

---

## Assignment 2: Intermediate Python Exercises

### Objective
In the second assignment, students practice more advanced Python features such as function definition, list comprehension, and handling mixed data types.

### Tasks and Solutions
1. **FizzBuzz Function**  
   Write a function `fizzbuzz(n)` that prints "Fizz" for multiples of 3, "Buzz" for multiples of 5, and "FizzBuzz" for multiples of both. For other numbers, print the number itself.

2. **Basic Data Filtering**  
   Create a list with mixed data types (integers, strings, floats) and filter only the integers using list comprehension.

3. **Simple To-Do List**  
   Implement a simple to-do list with functions to add tasks and show the list of tasks.

4. **Temperature Converter**  
   Write a function to convert temperatures from Celsius to Fahrenheit and print the converted values for given temperatures.

---

## Assignment 3: Object-Oriented Programming

### Objective
This assignment introduces the principles of object-oriented programming (OOP) and demonstrates how to create classes, objects, and methods in Python.

### Tasks and Solutions
1. **Student Class Implementation**  
   Students create a `Student` class with attributes for name, student ID, and a list of courses. Each course contains information about its name, grade, and credits. The class includes two methods: one for calculating the GPA based on the grades and credits of the courses, and another for printing student information.

   - **GPA Calculation**: The GPA is calculated by summing the total points for all courses (where points are the product of the course grade and credits) and dividing by the total number of credits.
   - **Student Info Display**: The student’s name, ID, GPA, and list of courses (with grades) are printed in a formatted way.

   The implementation demonstrates how OOP principles like encapsulation and object management can be applied to handle student data effectively.

---

## Assignment 4: Organizing and Analyzing Annotation Files

### Objective
This assignment focuses on processing and analyzing a collection of annotation files based on naming conventions. Key concepts include working with file operations, sorting, grouping, and performing aggregations using Python. The assignment also introduces modular and structured approaches to handle datasets effectively.

### Tasks and Solutions
1. **Identify incorrectly formatted files**  
   Process a directory of annotation files to identify and count files that do not conform to the expected naming convention. Extract correctly formatted files for further analysis.

2. **Group annotations by month**  
   Extract the date component from the filenames, identify the month, and group files into separate folders based on their month. Use Python’s `os` and `shutil` modules to create directories and move files.

3. **Count unique satellites**  
   Extract the satellite identifier from the filenames, determine the total number of unique satellites, and count the number of annotations for each satellite.

4. **Find the most frequently annotated satellite**  
   Identify the satellite with the highest number of annotations by comparing counts, and display the results.

5. **Count unique regions**  
   Extract and analyze the region information from filenames, identify unique regions, and determine their count.

6. **Sort and display filenames**  
   Sort the filenames in reverse order and print them in their original format to ensure that the sorting process is working as expected.

7. **Identify the most annotated month**  
   Analyze the grouped annotations to find the month with the highest number of files and display the corresponding results.

### Learning Outcomes
- Gain experience with Python file operations using modules like `os` and `shutil`.
- Practice data extraction, processing, and analysis using lists, sets, and dictionaries.
- Develop skills in grouping and organizing files programmatically.
- Enhance problem-solving abilities by applying structured approaches to data analysis tasks.

---

## Assignment 5: Data Analysis and File Handling

### Objective
In this assignment, students worked on data analysis tasks involving file handling, datetime manipulation, and dictionary-based storage. The focus was on understanding how to manage and process data efficiently, particularly in relation to file handling and analysis of timestamped data.

### Tasks and Solutions

1. **Analyze Annotations by Date**  
   The task required processing annotation files stored in a specific directory. The objective was to extract the date and time from each file's name, aggregate the annotations by year and month, and identify the month with the most annotations.

   - The solution involved reading filenames, using regex to parse the dates, and using Pandas to group and visualize the data.
   - A bar plot was generated to visually show the number of annotations per month and year, and the month with the most annotations was identified.

2. **Create and Save Data as JSON and Pickle**  
   Students were tasked with creating a dictionary where each key represented a month, and the corresponding value was a list of annotation names occurring in that month. They were then asked to save the data both in JSON and Pickle formats and later reload and verify the data.

   - The solution involved iterating over the annotation files, extracting relevant metadata (including date), and organizing the data by month.
   - The data was saved in JSON format, and then loaded back to verify its integrity. Additionally, the data was stored using Python's Pickle module for serialization.

3. **Sort Annotations for the Second Half of 2024**  
   The third task involved filtering annotation files from the second half of 2024 (from July to December), sorting them by date from oldest to newest, and printing the sorted list.

   - The solution involved parsing the datetime from the filenames, filtering for files from July to December 2024, and sorting them by date.
   - The final list of annotations was printed in chronological order.

---
## Assignment 6: Titanic Dataset Analysis

### Objective
In this assignment, students worked with the Titanic dataset to perform common data analysis tasks such as handling missing values, feature engineering, and filtering data. The goal was to practice data cleaning and transformation techniques that are often encountered in real-world data science projects.

### Tasks and Solutions

1. **Handle Missing Values**  
   Students were required to analyze the dataset for missing values in each column and implement strategies to fill in or handle the missing data. For example, they filled missing values in numerical columns with statistical measures like the mean and filled categorical columns with the most frequent value.

2. **Feature Engineering**  
   A new feature (column) was created to provide additional insights into the dataset. In this case, students added a column to indicate the family size of each passenger. This was done by summing the number of siblings/spouses (`SibSp`) and parents/children (`Parch`) on board.

3. **Data Filtering**  
   The task involved filtering passengers based on specific criteria, such as those who paid a fare above the average fare. This demonstrated the ability to analyze data subsets based on calculated or given thresholds.

4. **Basic Data Exploration**  
   Several basic data exploration steps were carried out, such as counting missing values, identifying common trends, and understanding the structure of the dataset. This helped in the overall data cleaning process and set the foundation for more advanced analysis.

### Libraries Used
- Pandas
- NumPy

---