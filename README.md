# chapter-no-4-self-
Self –Review Exercises
4.1 Answer each of the following questions.
a) All programs can be written in terms of three types of control structures: Sequence,  selection and repetition .
b) The  if …..else . selection statement is used to execute one action when a condition is true or a different action when that condition is false.
c) Repeating a set of instructions a specific number of times is called  Counter-controlled or definite   repletion.
d) When it isn't known in advance how many times a set of statements will be repeated, a(n) Sentinel,signal,flag or dummy  value can be used to terminate the repetition.
4.2 Write four different C++ statements that each add 1 to integer variable x.
× = × +1;
× += 1;
++×;
×++;
4.3 Write C++ statements to accomplish each of the following:
a) In one statement, assign the sum of the current value of x and y to z and postincrement the value of x.
 z = ×++  +  y
b) Determine whether the value of the variable count is greater than 10. If it is, print "Count is greater than 10." 
If ( count > 10 ) 
 Cout  << “ count is greater than 10 “ << end1;
c)  Predecrement the variable x by 1, then subtract it from the variable total.
  Total -= --×;
d) Calculate the remainder after q is divided by divisor and assign the result to u. Write this statement two different ways.
q %=  divisor ;
q =q% divisor;
4.4 Write C++ statements to accomplish each of the following tasks.
a) Declare variables sum and x to be of type int.
int sum ;
int x;
b) Set variable x to 1.
X = 1;
c) Set variable sum to 0.
Sum = 0;
d) Add variable x  to variable sum and assign the result to variable sum.
Sum += x; or sum = sum + x;
e) Print "The sun is: "followed by the value of variable sum. 
Cout <<” The sum is:” << sum <<end1;
4.5 Combine the statements that you wrote in Exercise 4.4 into a program that calculates and prints the sum of the integers from 1 to 10. Use the while statement to loop through the calculation and increment statements. The loop should terminate when the value of x becomes 11.
#include <iostream>
using namespace std;
int main()
{ int sum; // stores sum of integers 1 to 10 
 Int x; // counter 
X = 1 ;// count from 1 
Sum = 0; // initialize sum 
While ( x < = 10 ) // loop 10 times 
{ 
Sum += x ;// add x to sum 
++ x; // increment x 
} // end while 
Cout << “ The sum is :” << sum << end1;
}// end main 
Output :
The sum is : 55
4.6 State the values of each variable after the calculation is performed. Assume that, when each statement begins executing, all variables have the integer value 5.

a) product*= x++;
product = 25, x=6;
b) quotient/= ++x;
quotient = 0, x= 6 ;
#include <iostream>
using namespace std;
int main()
{ int x = 5;
Int product = 5;
Int quotient = 5;
// part a 
Product *= x++; // part a statement 
Cout << “ Value of product after calculation :”<< product << end1;
Cout <<”Valuse of x after calculation :” << x<< end1<< end1;
//part b
X= 5 ;// reset value of x 
Quotient /= ++x; // part b statement
Cout << “ Value of quotient after calculation :”<< quotient << end1;
Cout <<”Valuse of x after calculation :” << x<< end1<< end1;
} // end main
4.7 Write single C++ statements or portions of statements that do the following: 
a) Input integer variable x with cin and >>.
b) Input integer variable y with cin and >>.
c) Set integer variable i to 1.
d) Set integer variable power to 1.
e) Multiply variable power by x and assign the result to power.
f) Preincrement variable 1 by 1.
g ) Determine whether i is less than or equal to y.
 h)Output integer variable power with cout and <<.
Solution :
a) cin >> x;
b) cin >> y;

c) i = 1
d) power = 1;
e) power *= x ;
or
power= power * x;
f) ++i;
g) if (i <= y)
h) cout << power << endl;
4.8 Write a C++ program that uses the statements in Exercise 4.7 to calculate x raised to the y power. The program should have a while repetition statement.
1 // Exercise 4.8 Solution: ex04_08.cpp
2 // Raise x to the y power.
3 #include <iostream>
4 using namespace std;
5
6 int main()
7 {
8 int x; // base
9 int y; // exponent
10 int i; // counts from 1 to y
11 int power; // used to calculate x raised to power y
12
13 i=1; // initialize i to begin counting from 1
14 power 1; // initialize power
15
16 cout << "Enter base as an integer: "; // prompt for base
17 cin >> x; // input base
18
19 cout << "Enter exponent as an integer: "; // prompt for exponent
20 cin >> y; // input exponent
21
22 // count from 1 to y and multiply power by x each time
23 while (i <= y)
24 {
25 power *= x;
26 ++1;
27 } // end while
28
29 cout << power << endl; // display result
30 } // end main
Output:
Enter base as an integer : 2
Enter exponent as an integer :3
8
4.9Identify and correct the errors in each of the following:
a) while (c <= 5)
{
product *= c;
 ++C;
b) cin << value;
c) if (gender == 1 )
cout << "Woman" << endl;
else;
cout << "Man" << endl;
Solution:
a) Error: Missing the closing right brace of the while body.
Correction: Add closing right brace after the statement c++;.
b) Error: Used stream insertion instead of stream extraction.
Correction:Change << to >>.
c) Error: Semicolon after else results in a logic error. The second output statement will always be executed.
Correction:Remove the semicolon after else.
4.10 What's wrong with the following while repetition statement?
while (z >= 0)
sum += z;
Solution:
The value of the variable z is never changed in the while statement. Therefore, if the loop-continuation condition (z >= 0) is initially true, an infinite loop is created. To prevent the infinite loop, z must be decremented so that it eventually becomes less than 0.
