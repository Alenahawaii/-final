using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Task
{
    internal class Program
    {
        static void Main(string[] args)
        {
            string[] A = { "Hello", "World", "C#", "123456", "123", "Dog", "Cats" };
            Console.Write("Исходный массив строк: ");
            Console.WriteLine(string.Join(" ", A));
            int M = 0;
            for (int i = 0; i < A.Length; i++) if (A[i].Length <= 3) M++;
            string[] B = new string[M];
            int j = 0;
            for (int i = 0; i < A.Length; i++) if (A[i].Length <= 3) B[j++] = A[i];
            Console.Write("Новый массив строк: ");
            Console.WriteLine(string.Join(" ", B));
            Console.ReadKey();
        }
    }
}
