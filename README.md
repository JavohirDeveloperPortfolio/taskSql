# taskSql

## Task 1:

1. Create database University;

2. Create Tables:
    1. Student:
        - id bigint (Primary key)

        - name varchar

        - birthday date

        - group int

    2. Subject:

        - id bigint(Primary key)

        - name varchar

        - description varchar

        - grade int

    3. PaymentType:

        - id bigint(Primary key)

        - name varchar

    4. Payment:

        - id bigint(Primary key)

        - type_id bigint(FOREIGN KEY to PaymentType)

        - amount decimal

        - student_id bigint(FOREIGN KEY to Student)

        - payment_date datetime

    5. Mark

        - id bigint(Primary key)

        - student_id bigint(FOREIGN KEY to Student)

        - subject_id bigint(FOREIGN KEY to Subject)

        - mark int

## Task 2:

1) Insert new Students with names “John”, “Chris”, “Carl” for grade “1”, then with names “Oliver”, “James”, “Lucas” and
   “Henry” for grade “2” and with names “Jacob” and “Logan” for grade “3”. Insert more students for 4 and 5 grade.

2) Insert new Subjects:

- Art and music for 1 grade;
- Geography and history for 2 grade;
- PE and math for 3 grade;
- Science and IT for 4 grade.
- Insert 2 subjects for 5 grade.

3) Insert “DAILY”, “WEEKLY”, ”MONTHLY” Payment Types.

4) Insert 4 Payments:

- Payment is referenced to student with name “John” and “Weekly” payment type;
- Payment is referenced to student with name “Oliver” and “Monthly” payment type;
- Payment is referenced to student with name “Henry” and “Weekly” payment type
- Payment is referenced to student with name “James” and “Daily” payment type.
- Insert more payments for students.

5) Insert 5 Marks:

- 8 for Chris by Art;
- 5 for Oliver by History;
- 9 for James by Geography;
- 4 for Jacob by Math;
- 9 for Logan by PE.
- Insert more Masks for students.

 ## Task 3

1) Change table ‘Student’.
   ‘birthday’ field cannot be null
2) Change table ‘Mark’
   ‘mark’ should be in range from 1 to 10
   ‘student_id’ and ‘subject_id’ cannot be null
3) Change table ‘Subject’
   ‘grade’ should be in range from 1 to 5
4) Change table ‘PaymentType’
   ‘name’ should be a unique value
5) Change table ‘Payment’
   ‘type_id’, ‘amount’ and ‘date’ cannot be null

## Task 4:

1. Select all students with all the available fields
2. Select 50 students
3. Select only students’ name
4. Select unique values of Amount from Payment table
