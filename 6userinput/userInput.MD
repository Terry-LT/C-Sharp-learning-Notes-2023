# User Input
```cs
namespace My1Programm
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.Write("Write your name: ");
            String name = Console.ReadLine();
            Console.Write("Write your age: ");
            String age = Console.ReadLine();//or int age = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine(name);
            //Check if age is int
            int x = 0;
            if (int.TryParse(age,out x))
            {
                Console.WriteLine(x);
            }
            else
            {
                Console.WriteLine("Age only can be int");
            }

        }
    }
} 
```