# Abstract Class
```cs
using System.Runtime.CompilerServices;
using System.Security.Cryptography.X509Certificates;

namespace LearningCsharp
{
    class Program
    {
        public static void Main(string[] args)
        {
            //abstract class - modifier that indicates missing component or incomplete implements

            Car car = new Car(300, 4);
            Bicycle bicycle = new Bicycle(30, 2);
            Boat boat = new Boat(35, 0);
            //We want use to use specific vehicle. For example, car, bicycle, boat
            //But user can call class Vehicle. It is like choosing invisible cars
            //To prevent this class, we need add abstract to class Vehicle
            //now if we try to call this class, it will cause errors
            Vehicle vehicle = new Vehicle();
        }
        abstract class Vehicle
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
            public Car(int speed, int wheels)
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