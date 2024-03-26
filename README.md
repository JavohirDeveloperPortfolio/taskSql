# taskSql

## Lesson 1 tasks:

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
