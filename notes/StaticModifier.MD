# Static Modifier
```cs
using System.Runtime.CompilerServices;
using System.Security.Cryptography.X509Certificates;

namespace LearningCsharp
{
    class Program
    {
        public static void Main(string[] args)
        {
            //TODO: Continue Static
            //TODO: Add to github Static.MD
            //static = modifer to declare a static member which cannot be instantiated
            //You cannot create an object of a static class and cannot access static members using an object.

            CarNotStaticExample carNotStaticExample1 = new CarNotStaticExample("Mercedes");
            CarNotStaticExample carNotStaticExample2 = new CarNotStaticExample("Mustang");
            Console.WriteLine(carNotStaticExample1.numberOfCars);//Output is 1 
            Console.WriteLine(carNotStaticExample2.numberOfCars);//Ouput is 1
            //The value of numberOfCars did not increase
            //Let's try use static modifer
            CarStaticExample carStaticExample1 = new CarStaticExample("Mercedes");
            CarStaticExample carStaticExample2 = new CarStaticExample("Mustang");
            Console.WriteLine(CarStaticExample.numberOfCars);//Output is 2
            //It is possible to create a static method and call it from class directly
            //Smth like: CarStaticExample.SomeMethod();
            //Class can be also static
            ExStatic.hello();
            ExStatic.hello();
            //But you cannot declare it smth like
            //ExStatic exStatic = new ExStatic();


        }
        class CarNotStaticExample
        {
            string model;//default private
            public int numberOfCars;
            public CarNotStaticExample(String model)
            {
                this.model = model;
                numberOfCars += 1;
            }
        }
        class CarStaticExample
        {
            string model;//default private
            public static int numberOfCars;
            public CarStaticExample(String model)
            {
                this.model = model;
                numberOfCars += 1;
            }
        }
        public static class ExStatic
        {
            public static void hello()
            {
                Console.WriteLine("Hello!");
            } 
        }


    }
}
```