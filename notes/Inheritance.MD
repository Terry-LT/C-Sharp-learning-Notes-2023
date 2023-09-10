# Inheritance
```cs
using System.Runtime.CompilerServices;
using System.Security.Cryptography.X509Certificates;

namespace LearningCsharp
{
    class Program
    {
        public static void Main(string[] args)
        {
            //inheritance  = 1 or more child classes recieving fields, methods, etc. from a common parent
            Car car = new Car(300,4);
            Bicycle bicycle = new Bicycle(30, 2);
            Boat boat = new Boat(35, 0);

            Console.WriteLine(car.speed);
            Console.WriteLine(car.wheels);
            car.go();

            Console.WriteLine(bicycle.speed);
            Console.WriteLine(bicycle.wheels);
            bicycle.go();

            Console.WriteLine(boat.speed);
            Console.WriteLine(boat.wheels);
            boat.go();

        }
        class Vehicle
        {
            public int speed = 0;
            public int wheels = 0;
            public void go()
            {
                Console.WriteLine("This vehicle is moving!");
            }
        }
        class Car : Vehicle
        {
            public Car(int speed,int wheels)
            {
                this.speed = speed;
                this.wheels = wheels;
            }
        }
        class Bicycle : Vehicle
        {
            public Bicycle(int speed, int wheels)
            {
                this.speed = speed;
                this.wheels = wheels;
            }
        }
        class Boat : Vehicle
        {
            public Boat(int speed, int wheels)
            {
                this.speed = speed;
                this.wheels = wheels;
            }
        }



    }
}
```