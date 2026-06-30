## **Q2. Data Analytics Pipeline Algorithm**

**(Pseudocode for Student Performance Analytics Pipeline)**

**Input:** `student_data.csv` (Tabular data containing student IDs, names, course enrollments, task scores, attendance records, etc.)

**Process:**

**Data Analytics Pipeline Algorithm (Pseudocode for Student Performance Analysis)**

**Input:** `student_data.csv` containing student ID, name, department, attendance, diary entries, completed tasks, assignment marks, and lab marks.

```
START

Load the student dataset.

Check if the dataset is available.
If the file is missing or any required column is not found,
    display an error message and stop the program.

For each student record:

    Check for missing values.
    If any numeric value is missing,
        replace it with 0.

    Calculate the readiness score using the given performance values.

    If readiness score is less than 45,
        set Band = "Support"
    Else if readiness score is less than 70,
        set Band = "Developing"
    Else if readiness score is less than 90,
        set Band = "Strong"
    Else
        set Band = "Excellent"

    Save the readiness score and performance band.

Group all students according to their department.

Find the average readiness score for each department.

Identify the student with the highest readiness score.

Create a separate list of students whose band is "Support".

Display the following results:
1. Updated dataset with readiness score and band.
2. Department-wise average readiness score.
3. Details of the top-performing student.
4. List of students who need support.
5. Three observations based on the analysis.

END
```

