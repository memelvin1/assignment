# assignment
  static void Main(string[] args)
        {
            Rectangle r = new Rectangle();
            bool validrectangleselect = false;
            string rectangleselection;
            int selection;
            while (validrectangleselect == false)
            {
                Console.WriteLine("1.create default rectangle");
                Console.WriteLine("2.create custom rectangle");
                Console.WriteLine("choose a menu item to begin");
                rectangleselection = Console.ReadLine();
                Console.WriteLine();

                if (rectangleselection != "1" && rectangleselection != "2")
                {
                    Console.WriteLine("that is not a valid selection,please try again.\n");
                }
                else if (int.Parse(rectangleselection) == 1)
                {
                    validrectangleselect = true;
                    Random measure = new Random();
                    int length;
                    int width;
                    length = measure.Next(1, 1000);
                    width = measure.Next(1, 1000);
                    Console.WriteLine($"your values are {length}and{width}.\n");
                    Rectangle customrectangle = new Rectangle(length, width);
                    r = customrectangle;
                }
                else if (int.Parse(rectangleselection) == 2)
                {
