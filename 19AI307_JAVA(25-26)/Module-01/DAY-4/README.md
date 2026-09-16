# Ex.No:1(D) ARRAYS

## QUESTION:
Write a Java program to check whether an element appears more than once in an array.

## AIM:
To write a Java program that uses arrays and a data structure (HashSet) to check if any element is repeated in the given array.

## ALGORITHM :
1. Start the program.
2. Import the java.util package.
3. Read the size of the array (n) from the user.
4. Create an integer array of size n.
5. Read n elements from the user and store them in the array.
6. Create a HashSet to track seen elements.
7. Traverse each element in the array.
8. If an element is already in the HashSet, mark duplicate as true and stop checking.
9. Otherwise, add the element to the HashSet.
10. After traversal, if a duplicate was found, print "Yes"; otherwise print "No".
11. End the program.



## PROGRAM:
 ```
/*
Program to implement a Array concept using Java
Developed by: Priyanka S
RegisterNumber:  212224040255
*/
```

## SOURCE CODE:

```
import java.util.*;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        for(int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        boolean duplicate = false;
        Set<Integer> seen = new HashSet<>();
        for(int num : arr) {
            if(seen.contains(num)) {
                duplicate = true;
                break;
            }
            seen.add(num);
        }

        if(duplicate)
            System.out.println("Yes");
        else
            System.out.println("No");
    }
}



```





## OUTPUT:

<img width="610" height="726" alt="image" src="https://github.com/user-attachments/assets/a2f1dfdf-35db-4c77-a9cf-005c029da767" />



## RESULT:
  Thus, the Java program was successfully written and executed to check whether any element appears more than once in an array.
