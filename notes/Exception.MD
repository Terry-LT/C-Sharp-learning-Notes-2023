# Exception
```cs
namespace LearningCsharp
{
    class Program
    {
        public static void Main(string[] args)
        {
            try
            {
                Console.WriteLine("Enter number 1:");
                int x = Convert.ToInt32(Console.ReadLine());

                Console.WriteLine("Enter number 2:");
                int y = Convert.ToInt32(Console.ReadLine());

                Console.WriteLine(x / y);
            }
            catch (FormatException e)
            {
                Console.WriteLine(e.Message);
            }
            catch (DivideByZeroException e)
            {
                Console.WriteLine(e.Message);
            }
            catch (Exception e)
            {
                Console.WriteLine(e.Message + e.StackTrace);
            }
            finally
            {
                Console.WriteLine("Thanks. Good bye!");
            }
        }
 
    }
}
```