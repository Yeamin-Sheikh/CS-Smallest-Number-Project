# CS-Smallest-Number-Project
A github repository for practicing finding the smallest number among the 3
## Main Code  
```
using System;

namespace smallest_Number
{
    internal class Program
    {
        static void Main(string[] args)
        {
            try
            {
                Console.WriteLine("---FINDING THE SMALLEST NUMBER---");

                int n1, n2, n3, smallest;
                Console.Write("Enter the first number: ");
                n1 = Convert.ToInt32(Console.ReadLine());
                Console.Write("Enter the second number: ");
                n2 = Convert.ToInt32(Console.ReadLine());
                Console.Write("Enter the thrid number: ");
                n3 = Convert.ToInt32(Console.ReadLine());

                smallest = n1 < n2 && n1 < n3 ? n1 : n2 < n3 ? n2 : n3;

                Console.WriteLine("Among {0}, {1} and {2} the smallest number is {3}", n1, n2, n3, smallest);
            }
            catch (FormatException e)
            {
                Console.WriteLine("Enter Only Numbers Please!");
            }
            catch (Exception)
            {
                Console.WriteLine("Something Went Wrong!");
            }
            finally
            {
                Console.WriteLine("Press any key to exit.");
                Console.ReadKey();
            }
        }
    }
}
```
