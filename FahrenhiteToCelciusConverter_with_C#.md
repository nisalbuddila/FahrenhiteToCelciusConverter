# FahrenhiteToCelciusConverter
This is how to convert fahrenhite into celcius in c#


using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApplication4
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.Write("Enter Your Body Temperature(Fahrenheit):");
            double Fahrenheit = float.Parse(Console.ReadLine());
            double Celsius = (5.0 / 9.0) * (Fahrenheit - 32); 
            Console.WriteLine("Your body temperature in Celsius degrees is " + Math.Truncate(Celsius));
            if (37 < Celsius)
            {
                Console.WriteLine("You are ill!");
            }
            Console.ReadLine();
        }
    }
}
