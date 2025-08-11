1. Write a C# program to calculate the factorial of a given number using while
and for loop.

CODE:

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace kashish2
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Console.Write("Enter a number: ");
            int num = int.Parse(Console.ReadLine());

            int i = 1;
            long factorialWhile = 1;
            while (i <= num)
            {
                factorialWhile *= i;
                i++;
            }

            long factorialFor = 1;
            for (int j = 1; j <= num; j++)
            {
                factorialFor *= j;
            }

            Console.WriteLine($"\nFactorial of {num} using while loop: {factorialWhile}");
            Console.WriteLine($"Factorial of {num} using for loop: {factorialFor}");

            Console.ReadLine();
        }
    }
}


OUTPUT:  <img width="472" height="162" alt="image" src="https://github.com/user-attachments/assets/ca4ce4fd-fab5-40ae-a660-83d943e94784" />


OUTPUT:  <img width="472" height="162" alt="image" src="https://github.com/user-attachments/assets/ca4ce4fd-fab5-40ae-a660-83d943e94784" />
