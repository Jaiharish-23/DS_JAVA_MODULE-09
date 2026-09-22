# Ex17 Reversing a String Using Stack Data Structure
## DATE:17-09-2026
## AIM:
To write a Java program that reverses an input string using a stack, without using built-in reverse functions.

## Algorithm
1. Start the program.
2. Read the input string from the user.
3. Create an empty stack of characters.
4. Traverse the string and push each character onto the stack.
5. Pop each character from the stack and append it to a new string to obtain the reversed string.
6. Display the reversed string.
7. Stop the program. 

## Program:
```
/*
Program to reverses an input string using a stack
Developed by: JAI HARISH R
RegisterNumber:  212224040124
*/
```

```java

import java.util.Scanner;
import java.util.Stack;

public class ReverseStringWithStack {

    public static String reverseString(String input) {
         Stack<Character> stack=new Stack<>();
        for(char ch:input.toCharArray())
        {
            stack.push(ch);
        }
        StringBuilder rev=new StringBuilder();
        while(!stack.isEmpty())
        {
            rev.append(stack.pop());
        }
        return rev.toString();
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String input = scanner.nextLine();
        String reversed = reverseString(input);
        System.out.println(reversed);

        scanner.close();
    }
}


```

## Output:

<img width="446" height="156" alt="image" src="https://github.com/user-attachments/assets/b0e1ffbb-15d4-4cdc-91bc-7b1aa93294c8" />


## Result:
Thus, the program successfully reverses the given string using a stack without relying on built-in reverse functions.
