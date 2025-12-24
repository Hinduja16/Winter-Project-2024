# Winter-Project-2024# Student Result Management System (Java)

This repository contains a console-based **Student Result Management System** implemented in Java.  
The application lets you add student details, store them in a text file, compute totals and grades, and display all stored results.

## Features

- Add student result:
  - Roll number
  - Name
  - Marks in 3 subjects (`m1`, `m2`, `m3`)
- Automatic calculations:
  - Total marks = `m1 + m2 + m3`
  - Grade based on total:
    - `A` : total ≥ 270
    - `B` : total ≥ 240 and < 270
    - `C` : total ≥ 180 and < 240
    - `F` : total < 180
- Store each record in `students.txt` using file I/O.
- Display all saved student results in a tabular format.

## Code structure

- `StudentResultManagement.java`
  - `class Student`  
    Holds roll, name, marks, total, and grade.
  - `static char calculateGrade(int total)`  
    Returns grade based on total marks.
  - `static void addStudent()`  
    Reads input using `Scanner`, calculates total and grade, and appends data to `students.txt` using `FileWriter` and `BufferedWriter`.
  - `static void displayStudents()`  
    Reads and prints all records from `students.txt` using `FileReader` and `BufferedReader`.
  - `public static void main(String[] args)`  
    Menu-driven loop:
    - `1` – Add Student Result  
    - `2` – Display All Results  
    - `3` – Exit  

## How to run

1. Ensure JDK is installed and configured.  
2. Save the code as `StudentResultManagement.java` in a folder.  
3. Open a terminal in that folder and compile:

