# Pattern

## Aim:
To write a C# program for a pascal's triangle.

## Equipment Required:
visual studio

## Algorithm:
Step 1: Start the program.

Step 2: Create a class and declare two variables rows,Val using integer datatype.

Step 3: Using nested for loop create a pascal's triangle.

Step 4: Stop the execution.

## Program:
### Developed by : JANANI R
### Register Number : 212221230039
```
using System;

namespace condition
{
    public class pascal
    {
        public static void Main(string[] args)
        {
            Console.WriteLine("Pascal's Triangle : ");
            int rows = 5, num = 1;
            for (int i = 0; i < rows; i++)
            {
                for (int k = 1; k < rows - i; k++)
                {
                    Console.Write(" ");
                }
                for (int j = 0; j <= i; j++)
                {
                    if (i == 0 || j == 0)
                    {
                        num = 1;
                    }
                    else
                    {
                        num = num * (i - j + 1) / j;
                    }
                    Console.Write(num + " ");


                }
                Console.WriteLine();
            }
        }
    }
}

```

## Output:
![Screenshot 2023-03-21 161718](https://user-images.githubusercontent.com/94288340/226587041-3cb62d52-3b2c-4ed6-b674-dcc20878f12e.png)

## Result:
Thus the C# program to print the pascal's triangle is executed successfully
