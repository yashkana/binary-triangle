# binary-triangle
using System;

namespace binary1
{
    class binary1
    {
        static void Main(string[] args)
        {
            int number, digit = 1;
            Console.WriteLine("\n enter the number of lines:");
            number = Convert.ToInt32(Console.ReadLine());
            for (int i = 1; i <= number; i++)
            {
                for (int space = number - i; space > 0; space--)
                {
                    Console.Write(" ");
                }
                for (int j = 0; j < i; j++)
                {
                    Console.Write(digit + " ");
                    digit = (digit == 1) ? 0 : 1;
                }
                Console.Write("\n");
            }
        }
    }
}
