#########################This is the Readme file of the C++ implementation of Quine McCluskey Program ##################
 Name of the student:Arpit Kumar Singh
 Roll No:13/CS/31
 B.Tech 3rd Semester

  This code is build and compiled on GCC 4.8.1 complier.

1. How to compile the program:
     To compile the program TDM GCC 4.8.1 or any other updated compiler will be required.



2. How to give the input to run the program
    On execution of the Program .
    a. Input the roll no 
    b. Input  the number of variables
    c. Input the number of minterms   ### number of minterms not generated randomly as the generated number can be very large 
                                      ### leading the program to execute after a long duration of time.
                                      ### if needed the no of minterms can also be generated randomly but it will take a very long time to execute
    d.Input any one option 1 to input the minterms manually and 2 to generate the minterms randomly.
       (if option 1 is selected input the required number of minterms one by one.)
   
3. Output of the Program.
     a.The generated or entered minterms are displayed.
     b.The prime implicants after each comparison are displayed  sequentially.
     c.Then two matrix are displayed.Their descriptions are:
            
            The first required columns are the groups of compared prime implicants.
            The next  n(number of variables) columns display the status of the binary form of compared prime implicants.(in the binary form 2 is 
                                                                                                                         displayed instead of "-")
            The next column displays the latest group no.(group no taken as according to the satisfy the algorithms).    
            The next column dislpays the cost of the respective prime implicants.
            The next column dislpays the status of comparison(1 for selected for comparison and 0 for not selected for comparison).
      d. The essential prime implicants are displayed.
      e. The non essential prime implicants are displayed.


Sample Test cases:

Roll No =31
Number of variables=5
Number of minterms=12
Minterms entered manually: 0 1 2 8 9 15 17 21 24 25 27 31

Output:
The minterms  are
0 1 2 8 9 15 17 21 24 25 27 31
The prime impicants after  1   comparisons

0 1
0 2
0 8
1 9
1 17
8 9
8 24
9 25
15 31
17 21
17 25
24 25
25 27
27 31
The prime impicants after  2   comparisons

0 1 8 9
1 9 17 25
8 9 24 25
The second last table

0 1 0 0 0 0 2 11 4 1
0 2 0 0 0 2 0 11 4 0
0 8 0 2 0 0 0 11 4 1
1 9 0 2 0 0 1 12 4 1
1 17 2 0 0 0 1 12 4 1
8 9 0 1 0 0 2 12 4 1
8 24 2 1 0 0 0 12 4 1
9 25 2 1 0 0 1 13 4 1
15 31 2 1 1 1 1 15 4 0
17 21 1 0 2 0 1 13 4 0
17 25 1 2 0 0 1 13 4 1
24 25 1 1 0 0 2 13 4 1
25 27 1 1 0 2 1 14 4 0
27 31 1 1 2 1 1 15 4 0
The last table

0 1 8 9 0 2 0 0 2 22 3 0
1 9 17 25 2 2 0 0 1 23 3 0
8 9 24 25 2 1 0 0 2 23 3 0

 The essential prime implicants are

A'B'C'E'
BCDE
AB'D'E
BC'D'

The non - essential prime implicants are

A'C'D'
ABC'E

Limitation:
1.The code is tested on windows 8.1 oprerating system.

              