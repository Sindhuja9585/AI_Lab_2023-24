# Ex.No: 6   Logic Programming – Factorial of number   
### DATE:                                                                            
### REGISTER NUMBER : 212222220047
### AIM: 
To  write  a logic program  to solve Towers of Hanoi problem  using SWI-PROLOG. 
### Algorithm:
1. Start the program
2.  Write a rules for finding solution of Towers of Hanoi in SWI-PROLOG.
3.  a )	If only one disk  => Move disk from X to Y.
4.  b)	If Number of disk greater than 0 then
5.        i)	Move  N-1 disks from X to Z.
6.        ii)	Move  Nth disk from X to Y
7.        iii)	Move  N-1 disks from Y to X.
8. Run the program  to find answer of  query.

### Program:
```
move(1,X,Y,_) :- 
   write('Move top disk from '), 
   write(X), 
   write(' to '), 
   write(Y), 
   nl. 
move(N,X,Y,Z) :- 
   N>1, 
   M is N-1, 
   move(M,X,Z,Y), 
   move(1,X,Y,_), 
   move(M,Z,Y,X).
```


### Output:

![318402723-3ea15f0c-abff-414c-ad43-e88fd03edaa2](https://github.com/Sindhuja9585/AI_Lab_2023-24/assets/122860624/4e9389e3-8fc7-433e-9b53-d78a91a85830)


### Result:
Thus the solution of Towers of Hanoi problem was found by logic programming.
