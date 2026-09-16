
# 📊 Data Analyzer and Transformer Program

A menu-driven Python application for entering, analyzing, filtering, sorting, and calculating statistics from a one-dimensional dataset.

---

## 📌 Table of Contents

- [Project Overview](#-project-overview)
- [Objectives](#-objectives)
- [Features](#-features)
- [Technologies Used](#-technologies-used)
- [Python Concepts Used](#-python-concepts-used)
- [How the Program Works](#-how-the-program-works)
- [Menu Options](#-menu-options)
- [Installation](#-installation)
- [How to Run](#-how-to-run)
- [Sample Input](#-sample-input)
- [Sample Output](#-sample-output)
- [Algorithm](#-algorithm)
- [Time Complexity](#-time-complexity)
- [Testing](#-testing)
- [Advantages](#-advantages)
- [Limitations](#-limitations)
- [Future Enhancements](#-future-enhancements)
- [Learning Outcomes](#-learning-outcomes)
- [Conclusion](#-conclusion)
- [Project Information](#-project-information)

---

# 📖 Project Overview

The **Data Analyzer and Transformer Program** is a Python-based, menu-driven application developed to perform different operations on a one-dimensional array of integer values.

The program allows the user to:

- Enter numerical data
- Display a summary of the dataset
- Calculate the factorial of a number
- Filter data using a threshold value
- Sort data in ascending or descending order
- Display dataset statistics
- Exit the program

This project demonstrates the practical implementation of fundamental Python programming concepts such as **lists, functions, loops, conditional statements, recursion, lambda functions, filter(), sorting, and built-in functions**.

---

# 🎯 Objectives

The main objectives of this project are:

1. To create an interactive menu-driven Python application.
2. To accept and store numerical data in a one-dimensional list.
3. To calculate basic statistical information from the dataset.
4. To demonstrate the use of user-defined functions.
5. To implement factorial calculation using recursion.
6. To demonstrate the use of lambda functions and `filter()`.
7. To sort data in ascending and descending order.
8. To practice loops and conditional statements.
9. To understand basic data analysis operations.
10. To develop a simple and user-friendly Python project.

---

# ✨ Features

## 1. Input Data

The user can enter multiple integer values separated by spaces.

### Example

```text
Enter data for 1D array (separated by spaces):
10 20 5 30 15
````

The data is converted into a Python list.

```python
arr = list(map(int, data.split()))
```

Result:

```text
[10, 20, 5, 30, 15]
```

---

## 2. Display Data Summary

This option displays basic information about the dataset.

It provides:

* Total number of elements
* Minimum value
* Maximum value
* Sum of all values
* Average value

### Example

```text
Data Summary:
- Total elements: 5
- Minimum value: 5
- Maximum value: 30
- Sum of all value: 80
- Average value: 16.0
```

---

## 3. Calculate Factorial

This option calculates the factorial of a number entered by the user.

The factorial is calculated using a **recursive function**.

### Example

For:

```text
5
```

The calculation is:

```text
5! = 5 × 4 × 3 × 2 × 1
5! = 120
```

### Recursive Function

```python
def factorial(n):
    if n == 0 or n == 1:
        return 1
    else:
        return n * factorial(n - 1)
```

### Output

```text
Factorial of 5 is: 120
```

---

## 4. Filter Data by Threshold

This option filters the dataset and displays values greater than the threshold entered by the user.

The program uses:

* `filter()`
* Lambda function

### Example

Dataset:

```text
[10, 20, 5, 30, 15]
```

Threshold:

```text
15
```

Result:

```text
[20, 30]
```

### Code Used

```python
filtered_data = list(filter(lambda x: x > threshold, arr))
```

---

## 5. Sort Data

The program provides two sorting options:

```text
1. Ascending
2. Descending
```

### Ascending Order

Example:

```text
Original Data:
[30, 10, 20, 5]

Sorted Data:
[5, 10, 20, 30]
```

Python code:

```python
sorted_arr = sorted(arr)
```

### Descending Order

Example:

```text
Original Data:
[30, 10, 20, 5]

Sorted Data:
[30, 20, 10, 5]
```

Python code:

```python
sorted_arr = sorted(arr, reverse=True)
```

---

## 6. Display Dataset Statistics

This option calculates and displays:

* Maximum value
* Minimum value
* Sum of all values
* Average value

The project demonstrates how these operations can be implemented using user-defined functions and loops.

### Example

For the dataset:

```text
[10, 25, 5, 40, 15]
```

The output is:

```text
maximum value :- 40
Minimum value :- 5
sum of all values :- 95
average of values 19.0
```

---

## 7. Exit Program

This option terminates the program.

### Output

```text
Thank you for using the Data Analyzer and Transformer Program. Goodbye!
```

---

# 🛠️ Technologies Used

| Technology             | Purpose                             |
| ---------------------- | ----------------------------------- |
| Python 3               | Main programming language           |
| Python List            | Storing dataset                     |
| Functions              | Performing specific operations      |
| Recursion              | Calculating factorial               |
| Lambda Function        | Filtering data                      |
| `filter()`             | Selecting values based on condition |
| `sorted()`             | Sorting dataset                     |
| Loops                  | Processing data                     |
| Conditional Statements | Menu selection                      |

---

# 🧠 Python Concepts Used

## 1. Variables

Variables are used to store values during program execution.

Examples:

```python
choice
data
arr
num
threshold
total
```

---

## 2. Lists

The dataset is stored using a Python list.

Example:

```python
arr = [10, 20, 30, 40]
```

---

## 3. Input Function

The `input()` function is used to accept information from the user.

Example:

```python
choice = int(input("Please enter your Choice:- "))
```

---

## 4. Type Conversion

The `int()` function converts user input into an integer.

Example:

```python
num = int(input("Enter a number: "))
```

---

## 5. Functions

User-defined functions are used to divide the program into smaller and reusable sections.

Examples:

```python
def factorial(n):
```

```python
def maximum():
```

```python
def minimum():
```

```python
def sum_values():
```

```python
def average():
```

---

## 6. Recursion

Recursion is a technique where a function calls itself.

The factorial function uses recursion:

```python
return n * factorial(n - 1)
```

The recursion stops when:

```python
if n == 0 or n == 1:
    return 1
```

---

## 7. Lambda Function

A lambda function is used to create a short anonymous function.

Example:

```python
lambda x: x > threshold
```

---

## 8. Filter Function

The `filter()` function is used to select elements according to a condition.

Example:

```python
filter(lambda x: x > threshold, arr)
```

---

## 9. Sorting

The built-in `sorted()` function is used to arrange the elements.

Ascending:

```python
sorted(arr)
```

Descending:

```python
sorted(arr, reverse=True)
```

---

## 10. Loops

A `while` loop is used to repeatedly display the menu.

```python
while True:
```

A `for` loop is used to process the elements of the dataset.

```python
for choice in arr:
```

---

## 11. Conditional Statements

The program uses `if`, `elif`, and `else` statements to perform different operations based on the user's choice.

Example:

```python
if choice == 1:
    ...
elif choice == 2:
    ...
else:
    ...
```

---

# 🔄 How the Program Works

The overall working of the program is:

```text
                 START
                   |
                   v
        Display Welcome Message
                   |
                   v
             Display Menu
                   |
                   v
          Take User's Choice
                   |
       +-----------+-----------+
       |           |           |
       v           v           v
   Input Data    Analyze     Transform
       |           |           |
       +-----------+-----------+
                   |
                   v
          Display Result
                   |
                   v
          Display Main Menu
                   |
                   v
             User selects
              Exit (7)
                   |
                   v
                  END
```

---

# 📋 Menu Options

The main menu contains seven options:

| Option | Operation                  | Description                                 |
| ------ | -------------------------- | ------------------------------------------- |
| 1      | Input Data                 | Enter and store dataset                     |
| 2      | Display Data Summary       | Display basic dataset information           |
| 3      | Calculate Factorial        | Calculate factorial using recursion         |
| 4      | Filter Data by Threshold   | Display values above threshold              |
| 5      | Sort Data                  | Sort data ascending/descending              |
| 6      | Display Dataset Statistics | Calculate maximum, minimum, sum and average |
| 7      | Exit Program               | Close the application                       |

---

# 💻 Installation

## Requirements

Before running the project, make sure that Python 3.x is installed on your computer.

Check Python installation using:

```bash
python --version
```

or:

```bash
python3 --version
```

No external Python libraries are required for the basic program.

---

# ▶️ How to Run

### Step 1

Save the Python program as:

```text
data_analyzer.py
```

### Step 2

Open Command Prompt or Terminal.

### Step 3

Navigate to the folder where the Python file is saved.

### Step 4

Run the program:

```bash
python data_analyzer.py
```

The program will display:

```text
Welcome to the Data Analyzer and Transformer Program:

Main Menu:-

1. Input Data
2. Display Data Summary
3. Calculate Factorial
4. Filter Data by Threshold
5. Sort Data
6. Display Dataset Statistics
7. Exit Program
```

---

# 🧪 Sample Input

Suppose the user enters:

```text
10 25 5 40 15
```

The dataset becomes:

```text
[10, 25, 5, 40, 15]
```

---

# 📊 Sample Output

## Data Summary

```text
Data Summary:
- Total elements: 5
- Minimum value: 5
- Maximum value: 40
- Sum of all value: 95
- Average value: 19.0
```

## Factorial

```text
Enter a number to calculate its factorial: 5

Factorial of 5 is: 120
```

## Filter

For threshold `15`:

```text
Filtered data: [25, 40]
```

## Ascending Sort

```text
Sorted Data in Ascending Order:
[5, 10, 15, 25, 40]
```

## Descending Sort

```text
Sorted Data in Descending Order:
[40, 25, 15, 10, 5]
```

## Statistics

```text
maximum value :- 40
Minimum value :- 5
sum of all values :- 95
average of values 19.0
```

---

# 🧮 Algorithm

## Algorithm for Input Data

1. Start the program.
2. Display the main menu.
3. Select option 1.
4. Accept numbers separated by spaces.
5. Split the input into individual values.
6. Convert the values into integers.
7. Store the values in a list.
8. Display the stored data.
9. Return to the main menu.

---

## Algorithm for Data Summary

1. Check the stored dataset.
2. Count the number of elements.
3. Find the minimum value.
4. Find the maximum value.
5. Calculate the sum.
6. Calculate the average.
7. Display the results.

---

## Algorithm for Factorial

1. Accept a number from the user.
2. Check whether the number is 0 or 1.
3. If yes, return 1.
4. Otherwise, multiply the number by factorial of `n - 1`.
5. Continue until the base condition is reached.
6. Display the result.

---

## Algorithm for Filtering

1. Accept a threshold value.
2. Compare every dataset value with the threshold.
3. Select values greater than the threshold.
4. Store the selected values.
5. Display the filtered dataset.

---

## Algorithm for Sorting

1. Select sorting option.
2. If ascending is selected, sort from smallest to largest.
3. If descending is selected, sort from largest to smallest.
4. Display the sorted dataset.

---

# ⏱️ Time Complexity

Let `n` represent the number of elements in the dataset.

| Operation       | Time Complexity |
| --------------- | --------------- |
| Input Data      | O(n)            |
| Minimum         | O(n)            |
| Maximum         | O(n)            |
| Sum             | O(n)            |
| Average         | O(n)            |
| Filtering       | O(n)            |
| Ascending Sort  | O(n log n)      |
| Descending Sort | O(n log n)      |
| Factorial       | O(n)            |

---

# 🧪 Testing

The project should be tested with different inputs to ensure correct results.

## Test Case 1: Normal Dataset

### Input

```text
10 20 30 40 50
```

### Expected Result

```text
Minimum = 10
Maximum = 50
Sum = 150
Average = 30
```

---

## Test Case 2: Unsorted Dataset

### Input

```text
30 10 50 20 5
```

### Ascending Output

```text
[5, 10, 20, 30, 50]
```

### Descending Output

```text
[50, 30, 20, 10, 5]
```

---

## Test Case 3: Filtering

### Input

```text
10 20 30 40 50
```

### Threshold

```text
25
```

### Expected Output

```text
[30, 40, 50]
```

---

## Test Case 4: Factorial

### Input

```text
5
```

### Expected Output

```text
Factorial of 5 is: 120
```

---

## Test Case 5: Negative Values

### Input

```text
-10 -5 0 5 10
```

### Expected Result

```text
Minimum = -10
Maximum = 10
Sum = 0
Average = 0
```

---

# ⚠️ Error Handling

The current version of the program expects valid integer input.

For example:

```text
10 20 30 40
```

is valid.

However:

```text
10 abc 20
```

will cause an input conversion error because `abc` cannot be converted into an integer.

A future version can use `try-except` to handle invalid input.

The program can also be improved by checking whether data has been entered before options 2, 4, 5, and 6 are selected.

---

# ✅ Advantages

* Simple and easy to use.
* Menu-driven interface.
* Demonstrates multiple Python concepts.
* Performs several useful data operations.
* Uses functions to organize the program.
* Uses recursion for factorial calculation.
* Uses lambda and `filter()` for data filtering.
* Supports ascending and descending sorting.
* Provides basic statistical analysis.
* Suitable for learning Python fundamentals.

---

# ⚠️ Limitations

* The current program works mainly with integer values.
* Invalid input can cause an error.
* Data is not permanently stored after the program ends.
* The program does not currently read data from files.
* The dataset must be entered manually.
* There is no graphical user interface.
* Advanced statistical calculations are not included.

---

# 🚀 Future Enhancements

The project can be extended with the following features:

1. Add proper `try-except` error handling.
2. Add a check for empty datasets.
3. Support floating-point numbers.
4. Add median calculation.
5. Add mode calculation.
6. Add standard deviation.
7. Add variance calculation.
8. Add data visualization using Matplotlib.
9. Add CSV file import and export.
10. Save analysis results to a file.
11. Add a graphical user interface using Tkinter.
12. Add data validation.
13. Add search functionality.
14. Allow users to edit or delete dataset values.
15. Add a complete statistical report.

---

# 📈 Possible Advanced Version

In a future version, the project can become a complete data-analysis application with:

```text
Input Data
    ↓
Data Validation
    ↓
Data Cleaning
    ↓
Data Analysis
    ↓
Filtering
    ↓
Sorting
    ↓
Statistical Calculations
    ↓
Data Visualization
    ↓
Generate Report
```

---

# 🎓 Learning Outcomes

After completing this project, the following concepts are demonstrated:

* Python programming fundamentals
* Variables and data types
* Lists
* User input
* Type conversion
* `if-elif-else`
* `while` loops
* `for` loops
* User-defined functions
* Recursion
* Lambda functions
* `filter()`
* `sorted()`
* Built-in functions
* Basic statistics
* Data processing
* Menu-driven programming
* Algorithmic thinking
* Basic time-complexity analysis

---

# 🔍 Project Highlights

The major programming concepts demonstrated in this project are:

### 🔹 Data Storage

```python
arr = list(map(int, data.split()))
```

### 🔹 Recursion

```python
return n * factorial(n - 1)
```

### 🔹 Lambda Function

```python
lambda x: x > threshold
```

### 🔹 Filtering

```python
filter(lambda x: x > threshold, arr)
```

### 🔹 Sorting

```python
sorted(arr)
```

### 🔹 Reverse Sorting

```python
sorted(arr, reverse=True)
```

### 🔹 Looping

```python
for choice in arr:
```

### 🔹 Menu Loop

```python
while True:
```

---

# 📁 Suggested Project Structure

```text
Data-Analyzer-and-Transformer/
│
├── data_analyzer.py
│
├── README.md
│
└── screenshots/
    ├── main_menu.png
    ├── data_summary.png
    ├── factorial.png
    ├── filtering.png
    └── sorting.png
```

---

# 📸 Screenshots

Add screenshots of your running program in this section.

Recommended screenshots:

1. Main Menu
2. Input Data
3. Data Summary
4. Factorial Calculation
5. Filtered Data
6. Ascending Sorting
7. Descending Sorting
8. Dataset Statistics
9. Exit Message

Example:

```markdown
![Main Menu](screenshots/main_menu.png)
```

---

# 🔒 Data Privacy

This project processes the data entered by the user during program execution.

The current version does not send data to external servers or online services.

---

# 📜 License

This project is created for educational and academic purposes.

You are free to study, modify, and improve the source code for learning purposes.

---

# 👨‍💻 Project Information

| Detail               | Information                           |
| -------------------- | ------------------------------------- |
| Project Name         | Data Analyzer and Transformer Program |
| Programming Language | Python                                |
| Project Type         | Menu-Driven Application               |
| Data Structure       | One-Dimensional List                  |
| Difficulty Level     | Beginner / Intermediate               |
| Purpose              | Educational / Academic Project        |
| Interface            | Command Line / Console                |
| External Libraries   | None                                  |

---

# 🏆 Conclusion

The **Data Analyzer and Transformer Program** is a practical Python project that combines several fundamental programming concepts into one interactive application.

The program demonstrates how Python can be used to store, analyze, filter, transform, and organize numerical data.

Through this project, concepts such as **lists, functions, recursion, lambda functions, filtering, sorting, loops, conditional statements, and basic statistics** are applied in a practical situation.

The project also provides a strong foundation for developing more advanced data-analysis applications in the future.

---

# ⭐ Final Project Summary

```text
DATA ANALYZER AND TRANSFORMER PROGRAM

        INPUT
          ↓
       STORE DATA
          ↓
       ANALYZE DATA
          ↓
    ┌─────┼─────┐
    ↓     ↓     ↓
 FILTER  SORT  STATISTICS
    ↓     ↓     ↓
    └─────┼─────┘
          ↓
       DISPLAY
          ↓
         EXIT
```

---

## 📌 Keywords

```text
Python
Data Analyzer
Data Transformer
Data Analysis
Python Lists
Functions
Recursion
Lambda Function
Filter Function
Sorting
Statistics
Menu Driven Program
One Dimensional Array
Python Project
Academic Project
Beginner Python Project
```

---

# 🙏 Thank You

Thank you for using the **Data Analyzer and Transformer Program**.

**Developed using Python 🐍**

```
```

