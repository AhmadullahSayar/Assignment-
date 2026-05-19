# PL/SQL Student Assignments

## Student Information
- Name: Your Name
- Course: PL/SQL Programming
- Lecturer: M. Ghani Hussaini

---

# 1. Rectangle Area Program

```sql
DECLARE
    length NUMBER := 10;
    width NUMBER := 5;
    area NUMBER;
BEGIN
    area := length * width;

    DBMS_OUTPUT.PUT_LINE('Area of Rectangle = ' || area);
END;
/




2. Find Average of Three Numbers

DECLARE
    n1 NUMBER := 10;
    n2 NUMBER := 20;
    n3 NUMBER := 30;
    avg_num NUMBER;
BEGIN
    avg_num := (n1 + n2 + n3) / 3;z

    DBMS_OUTPUT.PUT_LINE('Average = ' || avg_num);
END;
/





complete this assignment in pl/sql language
PL/SQL Student Assignments
1. Create GitHub Account and Learn Git

Visit:

GitHub Official Website
Git Documentation

Basic Git Commands:

git init
git clone <repository-link>
git add .
git commit -m "first commit"
git push origin main
2. Rectangle Area Program
DECLARE
    length NUMBER := 10;
    width NUMBER := 5;
    area NUMBER;
BEGIN
    area := length * width;

    DBMS_OUTPUT.PUT_LINE('Area of Rectangle = ' || area);
END;
/
3. Find Average of Three Numbers
DECLARE
    n1 NUMBER := 10;
    n2 NUMBER := 20;
    n3 NUMBER := 30;
    avg_num NUMBER;
BEGIN
    avg_num := (n1 + n2 + n3) / 3;

    DBMS_OUTPUT.PUT_LINE('Average = ' || avg_num);
END;
/
4. Square Area Program
DECLARE
    side NUMBER := 4;
    area NUMBER;
BEGIN
    area := side * side;

    DBMS_OUTPUT.PUT_LINE('Area of Square = ' || area);
END;
/
5. Find the Average of Three Numbers
DECLARE
    a NUMBER := 15;
    b NUMBER := 25;
    c NUMBER := 35;
    average_num NUMBER;
BEGIN
    average_num := (a + b + c) / 3;

    DBMS_OUTPUT.PUT_LINE('Average = ' || average_num);
END;
/
6. Find the Largest Number among Three Numbers
DECLARE
    a NUMBER := 40;
    b NUMBER := 25;
    c NUMBER := 18;
BEGIN
    IF a >= b AND a >= c THEN
        DBMS_OUTPUT.PUT_LINE('Largest Number = ' || a);

    ELSIF b >= a AND b >= c THEN
        DBMS_OUTPUT.PUT_LINE('Largest Number = ' || b);

    ELSE
        DBMS_OUTPUT.PUT_LINE('Largest Number = ' || c);
    END IF;
END;
/
7. Find the Smallest Number among Three Numbers
DECLARE
    a NUMBER := 40;
    b NUMBER := 25;
    c NUMBER := 18;
BEGIN
    IF a <= b AND a <= c THEN
        DBMS_OUTPUT.PUT_LINE('Smallest Number = ' || a);

    ELSIF b <= a AND b <= c THEN
        DBMS_OUTPUT.PUT_LINE('Smallest Number = ' || b);

    ELSE
        DBMS_OUTPUT.PUT_LINE('Smallest Number = ' || c);
    END IF;
END;
/
8. Even and Odd Number Program
DECLARE
    num NUMBER := 7;
BEGIN
    IF MOD(num, 2) = 0 THEN
        DBMS_OUTPUT.PUT_LINE(num || ' is Even');

    ELSE
        DBMS_OUTPUT.PUT_LINE(num || ' is Odd');
    END IF;
END;
/
9. Simple Calculator Program (+, -, ×, ÷)
DECLARE
    a NUMBER := 20;
    b NUMBER := 5;
BEGIN
    DBMS_OUTPUT.PUT_LINE('Addition = ' || (a + b));
    DBMS_OUTPUT.PUT_LINE('Subtraction = ' || (a - b));
    DBMS_OUTPUT.PUT_LINE('Multiplication = ' || (a * b));
    DBMS_OUTPUT.PUT_LINE('Division = ' || (a / b));
END;
/
10. Celsius to Fahrenheit Conversion Program

Formula:

F=
5
9
	​

C+32

DECLARE
    celsius NUMBER := 30;
    fahrenheit NUMBER;
BEGIN
    fahrenheit := (celsius * 9/5) + 32;

    DBMS_OUTPUT.PUT_LINE('Fahrenheit = ' || fahrenheit);
END;
/
11. Student Grade Calculation Program
DECLARE
    marks NUMBER := 85;
BEGIN
    IF marks >= 90 THEN
        DBMS_OUTPUT.PUT_LINE('Grade = A');

    ELSIF marks >= 80 THEN
        DBMS_OUTPUT.PUT_LINE('Grade = B');

    ELSIF marks >= 70 THEN
        DBMS_OUTPUT.PUT_LINE('Grade = C');

    ELSIF marks >= 60 THEN
        DBMS_OUTPUT.PUT_LINE('Grade = D');

    ELSE
        DBMS_OUTPUT.PUT_LINE('Grade = F');
    END IF;
END;
/
12. Find the Sum of Numbers from 1 to 100

Formula:

S=
2
n(n+1)
	​


DECLARE
    sum_num NUMBER := 0;
    i NUMBER;
BEGIN
    FOR i IN 1..100 LOOP
        sum_num := sum_num + i;
    END LOOP;

    DBMS_OUTPUT.PUT_LINE('Sum = ' || sum_num);
END;
/
13. Find the Factorial of a Number
DECLARE
    num NUMBER := 5;
    fact NUMBER := 1;
    i NUMBER;
BEGIN
    FOR i IN 1..num LOOP
        fact := fact * i;
    END LOOP;

    DBMS_OUTPUT.PUT_LINE('Factorial = ' || fact);
END;
/
14. Electricity Bill Calculation Program
DECLARE
    units NUMBER := 250;
    bill NUMBER;
BEGIN
    IF units <= 100 THEN
        bill := units * 5;

    ELSIF units <= 200 THEN
        bill := (100 * 5) + ((units - 100) * 8);

    ELSE
        bill := (100 * 5) + (100 * 8) + ((units - 200) * 10);
    END IF;

    DBMS_OUTPUT.PUT_LINE('Electricity Bill = ' || bill);
END;
/
How to Run PL/SQL Programs

Enable output first:

SET SERVEROUTPUT ON;

Then run each program in Oracle SQL Developer or Oracle Database.

Recommended Software
Oracle SQL Developer
Oracle Database Express Edition (XE)
so how to upload  this assignment to my github

Here’s a simple step-by-step guide to upload your PL/SQL assignment to GitHub.

Step 1: Create a GitHub Account

Go to:

GitHub Official Website

Create your account and verify your email.

Step 2: Install Git

Download Git from:

Git Download Page

Install it with default settings.

Step 3: Create a New Repository on GitHub
Login to GitHub
Click New Repository

Repository name example:

plsql-assignment
Choose Public
Click Create Repository
Step 4: Create Your Assignment File

Open Notepad or VS Code and save your code as:

assignment.sql

Paste all your PL/SQL programs into this file.

You can also use:

Visual Studio Code
Step 5: Open Terminal / Git Bash

Go to the folder where assignment.sql is saved.

Right-click inside the folder and choose:

Git Bash Here
Step 6: Run Git Commands
Initialize Git
git init
Add Files
git add .
Commit Files
git commit -m "Added PL/SQL assignment"
Step 7: Connect Your GitHub Repository

Copy your repository URL from GitHub.

Example:

https://github.com/yourname/plsql-assignment.git

Now run:

git remote add origin https://github.com/yourname/plsql-assignment.git
Step 8: Upload to GitHub

Run:

git branch -M main
git push -u origin main

GitHub may ask for login authentication.

Step 9: Check Your Repository

Refresh your GitHub repository page.

You will see:

assignment.sql

uploaded successfully.

Optional: Add README File

Create a file named:

README.md

Example content:

# PL/SQL Assignment

Student Name: Your Name

This repository contains PL/SQL assignment programs.

Then upload again:

git add .
git commit -m "Added README"
git push
Helpful Tutorials
GitHub Docs
Git Tutorial for Beginners
in readme file
# PL/SQL Student Assignments

## Student Information
- Name: Your Name
- Course: PL/SQL Programming
- Lecturer: M. Ghani Hussaini

---

## Assignment List

1. Rectangle Area Program
2. Average of Three Numbers
3. Square Area Program
4. Largest Number among Three Numbers
5. Smallest Number among Three Numbers
6. Even and Odd Number Program
7. Simple Calculator Program
8. Celsius to Fahrenheit Conversion
9. Student Grade Calculation Program
10. Sum of Numbers from 1 to 100
11. Factorial of a Number
12. Electricity Bill Calculation Program

---

## Technologies Used

- Oracle Database
- PL/SQL
- Git & GitHub

---

## How to Run

1. Open Oracle SQL Developer
2. Enable server output:

```sql
SET SERVEROUTPUT ON;
Run the .sql file
GitHub Repository

This repository contains all PL/SQL assignment programs uploaded for academic purposes.

Author

Your Name

so do the the whole assignment create in readme file 
# PL/SQL Student Assignments

## Student Information
- Name: Your Name
- Course: PL/SQL Programming
- Lecturer: M. Ghani Hussaini

---

# 1. Rectangle Area Program

```sql
DECLARE
    length NUMBER := 10;
    width NUMBER := 5;
    area NUMBER;
BEGIN
    area := length * width;

    DBMS_OUTPUT.PUT_LINE('Area of Rectangle = ' || area);
END;
/
2. Find Average of Three Numbers
DECLARE
    n1 NUMBER := 10;
    n2 NUMBER := 20;
    n3 NUMBER := 30;
    avg_num NUMBER;
BEGIN
    avg_num := (n1 + n2 + n3) / 3;

    DBMS_OUTPUT.PUT_LINE('Average = ' || avg_num);
END;
/
3. Square Area Program
DECLARE
    side NUMBER := 4;
    area NUMBER;
BEGIN
    area := side * side;

    DBMS_OUTPUT.PUT_LINE('Area of Square = ' || area);
END;
/
4. Largest Number among Three Numbers
DECLARE
    a NUMBER := 40;
    b NUMBER := 25;
    c NUMBER := 18;
BEGIN
    IF a >= b AND a >= c THEN
        DBMS_OUTPUT.PUT_LINE('Largest Number = ' || a);

    ELSIF b >= a AND b >= c THEN
        DBMS_OUTPUT.PUT_LINE('Largest Number = ' || b);

    ELSE
        DBMS_OUTPUT.PUT_LINE('Largest Number = ' || c);
    END IF;
END;
/
5. Smallest Number among Three Numbers
DECLARE
    a NUMBER := 40;
    b NUMBER := 25;
    c NUMBER := 18;
BEGIN
    IF a <= b AND a <= c THEN
        DBMS_OUTPUT.PUT_LINE('Smallest Number = ' || a);

    ELSIF b <= a AND b <= c THEN
        DBMS_OUTPUT.PUT_LINE('Smallest Number = ' || b);

    ELSE
        DBMS_OUTPUT.PUT_LINE('Smallest Number = ' || c);
    END IF;
END;
/
6. Even and Odd Number Program
DECLARE
    num NUMBER := 7;
BEGIN
    IF MOD(num, 2) = 0 THEN
        DBMS_OUTPUT.PUT_LINE(num || ' is Even');

    ELSE
        DBMS_OUTPUT.PUT_LINE(num || ' is Odd');
    END IF;
END;
/
7. Simple Calculator Program
DECLARE
    a NUMBER := 20;
    b NUMBER := 5;
BEGIN
    DBMS_OUTPUT.PUT_LINE('Addition = ' || (a + b));
    DBMS_OUTPUT.PUT_LINE('Subtraction = ' || (a - b));
    DBMS_OUTPUT.PUT_LINE('Multiplication = ' || (a * b));
    DBMS_OUTPUT.PUT_LINE('Division = ' || (a / b));
END;
/
8. Celsius to Fahrenheit Conversion Program
DECLARE
    celsius NUMBER := 30;
    fahrenheit NUMBER;
BEGIN
    fahrenheit := (celsius * 9/5) + 32;

    DBMS_OUTPUT.PUT_LINE('Fahrenheit = ' || fahrenheit);
END;
/
9. Student Grade Calculation Program
DECLARE
    marks NUMBER := 85;
BEGIN
    IF marks >= 90 THEN
        DBMS_OUTPUT.PUT_LINE('Grade = A');

    ELSIF marks >= 80 THEN
        DBMS_OUTPUT.PUT_LINE('Grade = B');

    ELSIF marks >= 70 THEN
        DBMS_OUTPUT.PUT_LINE('Grade = C');

    ELSIF marks >= 60 THEN
        DBMS_OUTPUT.PUT_LINE('Grade = D');

    ELSE
        DBMS_OUTPUT.PUT_LINE('Grade = F');
    END IF;
END;
/
10. Sum of Numbers from 1 to 100
DECLARE
    sum_num NUMBER := 0;
    i NUMBER;
BEGIN
    FOR i IN 1..100 LOOP
        sum_num := sum_num + i;
    END LOOP;

    DBMS_OUTPUT.PUT_LINE('Sum = ' || sum_num);
END;
/
11. Factorial of a Number
DECLARE
    num NUMBER := 5;
    fact NUMBER := 1;
    i NUMBER;
BEGIN
    FOR i IN 1..num LOOP
        fact := fact * i;
    END LOOP;

    DBMS_OUTPUT.PUT_LINE('Factorial = ' || fact);
END;
/
12. Electricity Bill Calculation Program
DECLARE
    units NUMBER := 250;
    bill NUMBER;
BEGIN
    IF units <= 100 THEN
        bill := units * 5;

    ELSIF units <= 200 THEN
        bill := (100 * 5) + ((units - 100) * 8);

    ELSE
        bill := (100 * 5) + (100 * 8) + ((units - 200) * 10);
    END IF;

    DBMS_OUTPUT.PUT_LINE('Electricity Bill = ' || bill);
END;
/
Technologies Used
Oracle Database
PL/SQL
Git
GitHub
How to Run the Programs
SET SERVEROUTPUT ON;

Then run each PL/SQL block in Oracle SQL Developer.

GitHub Repository

This repository contains PL/SQL assignment solutions uploaded for academic purposes.

Author

Your Name

what is readme file

A README.md file is the main introduction file of a GitHub project or repository.

It explains:

What the project is
What programs/files are included
How to run the project
Who created it

GitHub automatically shows the README file on the front page of your repository.

Example Structure of a README File
# Project Title

Description of the project.

## Features
- Feature 1
- Feature 2

## How to Run
Instructions here.

## Author
Your Name
In Your Case

Your README.md contains:

Assignment title
PL/SQL programs
Technologies used
How to run the code
Your name

So when your teacher opens your GitHub repository, they immediately see all your assignment details.

Why .md?

README.md uses Markdown language.

Markdown helps format text like:

Headings
Bold text
Code blocks
Lists

Example:

# Big Heading
## Small Heading

**Bold Text**

```sql
SELECT * FROM students;

---

# How to Create README.md

Inside your project folder:

1. Right click
2. New File
3. Name it:

```text id="o92jfe"
README.md

Paste your assignment content inside it.

Example Repository Structure
plsql-assignment/
│
├── README.md
└── assignment.sql
Where It Appears on GitHub

When uploaded, GitHub automatically displays the README on the main repository page.

Learn more:

GitHub README Documentation
can i upload in notpad file

Yes, you can upload a Notepad file to GitHub.

If you wrote your assignment in Notepad, save it as either:

README.md

or

assignment.sql

Both can be uploaded to GitHub.

Option 1 — Recommended (README.md)

If you want the assignment to appear directly on the GitHub homepage, save the file as:

README.md

Steps:

Open Notepad
Paste the README content
Click File → Save As
In File Name, type:
README.md
Change Save as type to:
All Files
Click Save
Option 2 — SQL File

If you only want to upload the PL/SQL code, save as:

assignment.sql
How to Upload Directly on GitHub (Without Git Commands)
Open your repository on GitHub
Click:
Add file → Upload files
Drag your Notepad file there
Click:
Commit changes

Done — your file is uploaded.

Best Practice

Use both files:

README.md       → explanation + assignment display
assignment.sql  → actual PL/SQL code

This looks more professional on GitHub.

how i can create the file and then upload 
Step 1 — Create the File in Notepad
Create README.md
Open Notepad
Copy your assignment content
Paste it into Notepad

Now save the file:

Click File → Save As
In File name type:
README.md
In Save as type, choose:
All Files
Click Save

Your README file is now created.

Step 2 — Create GitHub Repository

Go to:

GitHub

Then:

Login
Click New Repository
Repository name example:
plsql-assignment
Click Create Repository
Step 3 — Upload the File

Inside your repository page:

Click:
Add file
Select:
Upload files
Drag your README.md file into GitHub
OR click:
choose your files

and select the file.

Step 4 — Commit the File

Scroll down.

In the message box type:

Added PL/SQL assignment

Then click:

Commit changes
Finished ✅

Your assignment is now uploaded to GitHub.

When someone opens your repository, the README file will automatically appear on the homepage.

Final Result Example
plsql-assignment/
└── README.md
Optional: Upload SQL File Too

You can also create another file:

assignment.sql

and upload it the same way.

so give the code 
# PL/SQL Student Assignments

## Student Information
- Name: Your Name
- Course: PL/SQL Programming
- Lecturer: M. Ghani Hussaini

---

# 1. Rectangle Area Program

```sql
DECLARE
    length NUMBER := 10;
    width NUMBER := 5;
    area NUMBER;
BEGIN
    area := length * width;

    DBMS_OUTPUT.PUT_LINE('Area of Rectangle = ' || area);
END;
/
2. Find Average of Three Numbers
DECLARE
    n1 NUMBER := 10;
    n2 NUMBER := 20;
    n3 NUMBER := 30;
    avg_num NUMBER;
BEGIN
    avg_num := (n1 + n2 + n3) / 3;

    DBMS_OUTPUT.PUT_LINE('Average = ' || avg_num);
END;
/
3. Square Area Program
DECLARE
    side NUMBER := 4;
    area NUMBER;
BEGIN
    area := side * side;

    DBMS_OUTPUT.PUT_LINE('Area of Square = ' || area);
END;
/



4. Largest Number among Three Numbers
DECLARE
    a NUMBER := 40;
    b NUMBER := 25;
    c NUMBER := 18;
BEGIN
    IF a >= b AND a >= c THEN
        DBMS_OUTPUT.PUT_LINE('Largest Number = ' || a);

    ELSIF b >= a AND b >= c THEN
        DBMS_OUTPUT.PUT_LINE('Largest Number = ' || b);

    ELSE
        DBMS_OUTPUT.PUT_LINE('Largest Number = ' || c);
    END IF;
END;
/



5. Smallest Number among Three Numbers
DECLARE
    a NUMBER := 40;
    b NUMBER := 25;
    c NUMBER := 18;
BEGIN
    IF a <= b AND a <= c THEN
        DBMS_OUTPUT.PUT_LINE('Smallest Number = ' || a);

    ELSIF b <= a AND b <= c THEN
        DBMS_OUTPUT.PUT_LINE('Smallest Number = ' || b);

    ELSE
        DBMS_OUTPUT.PUT_LINE('Smallest Number = ' || c);
    END IF;
END;
/


6. Even and Odd Number Program
DECLARE
    num NUMBER := 7;
BEGIN
    IF MOD(num, 2) = 0 THEN
        DBMS_OUTPUT.PUT_LINE(num || ' is Even');

    ELSE
        DBMS_OUTPUT.PUT_LINE(num || ' is Odd');
    END IF;
END;
/



7. Simple Calculator Program
DECLARE
    a NUMBER := 20;
    b NUMBER := 5;
BEGIN
    DBMS_OUTPUT.PUT_LINE('Addition = ' || (a + b));
    DBMS_OUTPUT.PUT_LINE('Subtraction = ' || (a - b));
    DBMS_OUTPUT.PUT_LINE('Multiplication = ' || (a * b));
    DBMS_OUTPUT.PUT_LINE('Division = ' || (a / b));
END;
/





7. Simple Calculator Program
DECLARE
    a NUMBER := 20;
    b NUMBER := 5;
BEGIN
    DBMS_OUTPUT.PUT_LINE('Addition = ' || (a + b));
    DBMS_OUTPUT.PUT_LINE('Subtraction = ' || (a - b));
    DBMS_OUTPUT.PUT_LINE('Multiplication = ' || (a * b));
    DBMS_OUTPUT.PUT_LINE('Division = ' || (a / b));
END;
/



8. Celsius to Fahrenheit Conversion Program
DECLARE
    celsius NUMBER := 30;
    fahrenheit NUMBER;
BEGIN
    fahrenheit := (celsius * 9/5) + 32;

    DBMS_OUTPUT.PUT_LINE('Fahrenheit = ' || fahrenheit);
END;
/





9. Student Grade Calculation Program
DECLARE
    marks NUMBER := 85;
BEGIN
    IF marks >= 90 THEN
        DBMS_OUTPUT.PUT_LINE('Grade = A');

    ELSIF marks >= 80 THEN
        DBMS_OUTPUT.PUT_LINE('Grade = B');

    ELSIF marks >= 70 THEN
        DBMS_OUTPUT.PUT_LINE('Grade = C');

    ELSIF marks >= 60 THEN
        DBMS_OUTPUT.PUT_LINE('Grade = D');

    ELSE
        DBMS_OUTPUT.PUT_LINE('Grade = F');
    END IF;
END;
/


10. Sum of Numbers from 1 to 100
DECLARE
    sum_num NUMBER := 0;
    i NUMBER;
BEGIN
    FOR i IN 1..100 LOOP
        sum_num := sum_num + i;
    END LOOP;

    DBMS_OUTPUT.PUT_LINE('Sum = ' || sum_num);
END;
/











11. Factorial of a Number
DECLARE
    num NUMBER := 5;
    fact NUMBER := 1;
    i NUMBER;
BEGIN
    FOR i IN 1..num LOOP
        fact := fact * i;
    END LOOP;

    DBMS_OUTPUT.PUT_LINE('Factorial = ' || fact);
END;
/













12. Electricity Bill Calculation Program
DECLARE
    units NUMBER := 250;
    bill NUMBER;
BEGIN
    IF units <= 100 THEN
        bill := units * 5;

    ELSIF units <= 200 THEN
        bill := (100 * 5) + ((units - 100) * 8);

    ELSE
        bill := (100 * 5) + (100 * 8) + ((units - 200) * 10);
    END IF;

    DBMS_OUTPUT.PUT_LINE('Electricity Bill = ' || bill);
END;
/















