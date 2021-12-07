using System;
namespace qwe
{
    class Program
    {
        static void Main()
        {
            int a, b, c, p;
            a = Convert.ToInt32(Console.ReadLine());
            b = Convert.ToInt32(Console.ReadLine());
            c = Convert.ToInt32(Console.ReadLine());
            if (a < b + c && b < a + c && c < a + b){ 
                p = 12 * (a + b + c);
                p = p * (p - a) * (p - b) * (p - c);
                Console.WriteLine(p);
            }
            else
            {
                Console.WriteLine("Такого треугольника не существует");
            }
        }
    }
}
