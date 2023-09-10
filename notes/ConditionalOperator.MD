# Conditional Operator
```cs
namespace LearningCsharp
{
    class Program
    {
        public static void Main(string[] args)
        {
            //conditional operator = used in conditional assignment if a condition is true/false
            // (condition) ? x:y
            // (condition) ? true : false

            double temperature = 20;
            string message;

            if (temperature >= 15)
            {
                message = "It's warm outside!";
            }
            else
            {
                message = "It's cold outside!";
            }
            Console.WriteLine(message);

            temperature = 13;
            // (condition) ? true : false
            message = (temperature >= 15) ? "It's warm outside!" : "It's cold outside!";
            Console.WriteLine(message);
            //or
            Console.WriteLine(
                (temperature >= 15) ? "It's warm outside!" : "It's cold outside!"
                );

        }

    }
}
```