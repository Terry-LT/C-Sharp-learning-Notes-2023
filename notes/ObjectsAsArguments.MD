# Objects as arguments
```cs
sing System.Runtime.CompilerServices;
using System.Security.Cryptography.X509Certificates;

namespace LearningCsharp
{
    class Program
    {
        public static void Main(string[] args)
        {
            Car car = new Car("camry",220);
            ChangeMaxSpeed(car, 200);
            Console.WriteLine(car.maxSpeed);
            Car car2 = CopyCar(car);
            car2.model = "corolla";
            Console.WriteLine(car2.model);
        }
        public static void ChangeMaxSpeed(Car car,int maxSpeed)
        {
            car.maxSpeed = maxSpeed;
        }
        public static Car CopyCar(Car car)
        {
            return new Car(car.model,car.maxSpeed);
        }
      
    }
    class Car
    {
        public string model;
        public int maxSpeed;
        public Car(string model, int maxSpeed)
        {
            this.model = model;
            this.maxSpeed = maxSpeed;
        }
        
    }
}
```