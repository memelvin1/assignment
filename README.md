# assignment
 else
                {
                    validMenuSelect = true;
                }

            }
            Console.WriteLine();
            return int.Parse(userInput);
        }
        public static int ValidateUserInput(string Side)
        {
            int number = 1;
            bool isValid = false;
            while (isValid == false)
            {
                Console.WriteLine("pls enter the {side} of your rectangle:");
                string userInput = Console.ReadLine();
                Console.WriteLine();
                bool result = int.TryParse(userInput, out number);
                if (result == false)
                {
                    Console.WriteLine("thats not a valid input,please try again:/n");
                }
                else if (number < 0)
                {
                    Console.WriteLine("number cannot be less than 0,please try again:/n");

                }
                else
                {
                    isValid = true;
                    object chosennumber = null;
                    Console.WriteLine($"your {chosennumber}has been changed to:{number}.\n");

                }
            }
            return number;
        }
