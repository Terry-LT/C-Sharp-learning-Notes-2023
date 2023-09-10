# Method over loading and param keyword
```cs
namespace LearningCsharp
{
    class Program
    {
        public static void Main(string[] args)
        {
            //method overloading = methods with the same name but different parameters
            double total;
            total = Multiply(2, 2);
            Console.WriteLine(total);

            double total2;
            total2 = Multiply(2, 2,3);
            Console.WriteLine(total2);
            //26th part
            //params keyword - it takes a variable number of arguments
            Console.WriteLine(
                Sum(1, 2, 3, 4, 5)
                );

        }
        public static double Sum(params double[] prices)
        {
            double totalPrice = 0;
            foreach (double price in prices){
                totalPrice += price;
            }
            return totalPrice;

        }
        public static double Multiply(double a, double b)
        {
            return a * b;
        }
        public static double Multiply(double a,double b, double c)
        {
            return a * b * c;
        }
    }
}
```