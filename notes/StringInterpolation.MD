# String Interpolation
```cs
namespace LearningCsharp
{
    class Program
    {
        public static void Main(string[] args)
        {
            String firstName = "Timur";
            String secondName = "Lora";
            int age = 19;
            Console.WriteLine($"Hello {firstName} {secondName}");
            //You cad space number or -number
            Console.WriteLine($"You are {age,10} old!");
        }

    }
}
```