# Ex.No:1(B) CONDITIONAL STATEMENT

## QUESTION:
Aliens scan DNA numbers:

If the DNA number is divisible by 2 and ends in 4, they accept it.

If the DNA number is divisible by 2 but ends in anything else, it’s a suspect.

If the DNA is odd, they reject it.

## For example:

```
---------------------------
Input	       Result 
64        |  Accepted
-----------------------------

```
## AIM:

To implement conditional logic in Java using nested if-else statements and the modulus operator to solve a classification problem.


## ALGORITHM :

1.Start the program.

2.Import the java.util.Scanner class for user input.

3.Create a Scanner object to read from the console.

4.Read the integer dnaNumber from the user.

5.Check if dnaNumber is even ( dnaNumber % 2 == 0 ).

6.If it is even, enter a nested check:

7.Check if dnaNumber ends in 4 ( dnaNumber % 10 == 4 ).

  - If true, print "Accepted".

  - If false, print "Suspect".

  - If the number is not even (it's odd), print "Rejected".

8. End the program.


## PROGRAM:
 ```

Program to implement a conditional statement using Java
Developed by:  Priyanka S
RegisterNumber:  212224040255

```

## SOURCE CODE:

```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int dnaNumber = scanner.nextInt();

        if (dnaNumber % 2 == 0) {
            if (dnaNumber % 10 == 4) {
                System.out.println("Accepted");
            } else {
                System.out.println("Suspect");
            }
        } else {
            System.out.println("Rejected");
        }

    }
}
```


## OUTPUT:

<img width="1235" height="476" alt="Screenshot 2025-11-16 123601" src="https://github.com/user-attachments/assets/d34b3a42-80cd-4c93-a256-f74f86f91358" />


## RESULT:


The program was successfully developed and executed.It correctly classifies the given DNA number as Accepted, Suspect, or Rejected based on the specified conditional rules.
