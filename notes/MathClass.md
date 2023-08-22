# Math Class
```cs
namespace My1Programm
{
    class Program
    {
        static void Main(string[] args)
        {
            //Power method
            double x = 3;
            double a = Math.Pow(x,2);//x^2 or x power of 2
            Console.WriteLine(a);// output will be 9
            //Basically the same but without Math class
            double b = 1;
            for (int i = 0;i <= x; i++)
            {
                b = x * x;
            }
            Console.WriteLine(b);// output will be 9

            //Sqr
            double c = Math.Sqrt(x);
            Console.WriteLine(c);// output will be 1.7320508075688772
            //Abs
            double y = -3;
            double d = Math.Abs(y);
            Console.WriteLine(d);// output will be positive 3

        }
    }
}
```