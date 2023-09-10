# Class and Object
```cs
using System.Security.Cryptography.X509Certificates;

namespace LearningCsharp
{
    class Program
    {
        public static void Main(string[] args)
        {
            //class - it is a data structure that can contain functions,variables
            //Can be used as a blueprint to create objects(OOP)
            Message.Hello();
            Message.Bye();
            //Object can have fields and methods (characteristics and actions)
            Human human1 = new Human("Tima", 19);
            Human human2 = new Human("Napo", 22);
            human1.Eat();
            human1.Sleep();
            human2.Eat();
            human2.Sleep();
        }
        public static class Message
        {
            public static void Hello()
            {
                Console.WriteLine("Hello");
            }
            public static void Bye()
            {
                Console.WriteLine("Bye");
            }
        }

        public class Human
        {
            private String name;
            private int age;
            public Human(String name, int age)
            {
                this.name = name;
                this.age = age;
            }
            public void Eat()
            {
                Console.WriteLine(name + "is eating");
            }
            public void Sleep()
            {
                Console.WriteLine(name + "is sleeping");
            }
        }

    }
}
```