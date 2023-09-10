# Array
```cs
namespace LearningCsharp
{
    class Program
    {
        public static void Main(string[] args)
        {
            String[] cars = { "BMW", "Nissan", "Toyota" };
            for (int i = 0; i < cars.Length; i++)
            {
                Console.WriteLine(cars[i]);
            }
            //update value from array
            cars[0] = "Tesla";
            Console.WriteLine("cars[0] is now " + cars[0]);
            Console.WriteLine("");
            //or
            for (int i = 0;i < cars.Length; i++)
            {
                if (cars[i] == "Tesla")
                {
                    cars[0] = "BMW";
                    Console.WriteLine("cars[0] is now " + cars[0]);
                }
            }
        }
    }
}
```