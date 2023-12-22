using System;

namespace FactorialCalculator
{
    class Program
    {
        static long Factorial(int n)
        {
            if (n == 0)
            {
                return 1;
            }
            
            if (n == 1)
            {
                return 1;
            }
            
            else
            {
                return n * Factorial(n - 1);
            }
        }

        static void Main(string[] args)
        {
            Console.Write("Введите число: ");
            int num = Convert.ToInt32(Console.ReadLine());
            long result = Factorial(num);
            Console.WriteLine($"Факториал числа {num} = {result}");
        }
    }
}
