# Ex.No: 5   Logic Programming – Factorial of number   
### DATE:                                                                            
### REGISTER NUMBER : 212222220047
### AIM: 
To  write  a logic program for finding the factorial of given number using SWI-PROLOG. 
### Algorithm:
1. STEP 1: Start the program
2. STEP 2:  Write a rules for finding factorial of given program in SWI-PROLOG.
3.   a)	factorial of 0 is 1 => written as factorial(0,1).
4.   b)	factorial of number greater than 0 obtained by recursively calling the factorial    function.
5. STEP 3: Run the program  to find answer of  query.
6. STEP 4: Stop the program.

### Program:
```
% Base case: factorial of 0 is 1
factorial(0, 1).
% Recursive case: factorial of A is B if A is greater than 0
factorial(A, B) :-
A > 0,
C is A - 1,
factorial(C, D),
B is A * D.
```


### Output:

![Screenshot 2024-03-11 161843](https://github.com/Sindhuja9585/AI_Lab_2023-24/assets/122860624/e7b419b3-6f60-4848-930b-c8ff66e60924)


### Result:
Thus the factorial of given number was found by logic programming. 
