 1. Rectangle Area Program

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
