# Ex.No:1(B) CONDITIONAL STATEMENT

## QUESTION:
You're entering a magical maze with a 3-digit access code. Based on its digits, the maze behaves differently:
-> If the middle digit is 0 → Maze freezes.
-> If the sum of digits is exactly 15 → Maze reflects you back.
-> If the first digit is odd and the last digit is even → Maze opens.
-> Otherwise → Maze collapses.

## AIM:
To write a Java program that reads a 3-digit access code and determines the behavior of a magical maze based on the conditions involving the digits—whether the maze freezes, reflects, opens, or collapses.

## ALGORITHM :
1.Start the program.
2.Import the necessary package 'java.util'
3.Read the 3-digit access code from the user.
4.Extract the digits:
first digit = code / 100
middle digit = (code / 10) % 10
last digit = code % 10
5.Check the conditions in order:
If the middle digit is 0, display “Maze freezes.”
Else if the sum of all digits is 15, display “Maze reflects you back.”
Else if the first digit is odd AND the last digit is even, display “Maze opens.”
Otherwise, display “Maze collapses.”
6.End the program.
	





## PROGRAM:
 ```
/*
Program to implement a conditional statement using Java
Developed by: Deepika R 
RegisterNumber: 212224040061 
*/
```

## SOURCE CODE:

```
import java.util.*;
public class Main
{
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);
        int num = sc.nextInt();
        int first = num / 100;
        int mid = (num / 10) % 10;
        int last = num % 10;
        int sum = first + mid + last;
        if(mid == 0)
        {
            System.out.print("Freezes");
        }
        else if(sum==15)
        {
            System.out.print("Reflects");
        }
        else if(first % 2 == 1 && last % 2 == 0)
        {
            System.out.print("Opens");
        }
        else
        {
            System.out.print("Collapses");
        }
    }
}
```







## OUTPUT:

<img width="442" height="286" alt="Screenshot 2026-09-03 160057" src="https://github.com/user-attachments/assets/9828cd6b-8678-4d65-a87e-1b1d2002a645" />


## RESULT:
Thus, the program was successfully written and executed. The behavior of the magical maze was correctly determined based on the digits of the 3-digit access code according to the given conditions.
