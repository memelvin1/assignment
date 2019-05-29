# assignment
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp9
{
    class Program
    {
        public static int validateMenuSelection()
        {

            string userInput = "";
            bool validMenuSelect = false;
            while (validMenuSelect == false)
            {
                Console.WriteLine("1.get rectangle length");
                Console.WriteLine("2.change rectangle length");
                Console.WriteLine("3.get rectangle width");
                Console.WriteLine("4.change rectangle width");
                Console.WriteLine("5.get rectangle perimeter");
                Console.WriteLine("6.get rectangle area");
                Console.WriteLine("7.exit");

                Console.WriteLine("please select an option,by entering a number:\n");
                userInput = Console.ReadLine();
                if (
                    userInput != "1" &&
                    userInput != "2" &&
                    userInput != "3" &&
                    userInput != "4" &&
                    userInput != "5" &&
                    userInput != "6" &&
                    userInput != "7"
                    )
                {
                    Console.WriteLine("thats not a valid menu option,pleasetry again");
                }
