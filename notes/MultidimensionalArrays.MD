# Multidimensional Arrays
```cs
namespace LearningCsharp
{
    class Program
    {
        public static void Main(string[] args)
        {
            String[] ford = { "Focus","Mustang","Escape"};
            String[] chevy = { "Chevrolet Cruze", "Chevrolet Suburban", "Equinox" };
            String[] toyota = { "Corolla", "Yaris", "GR Supra" };

            String[,] parkingLot =
            {
                { "Focus","Mustang","Escape"},//0 position, mustang is in 1 position
                { "Chevrolet Cruze", "Chevrolet Suburban", "Equinox" },//1 position, cruze is in 1 position
                { "Corolla", "Yaris", "GR Supra" }//2 position
            };
            parkingLot[0, 1] = "Update Mustang";
            parkingLot[1, 0] = "Just Updated Cruze :)";
            /*foreach (String car in parkingLot)
            {
                Console.WriteLine(car);
            }*/
            for (int i = 0; i < parkingLot.GetLength(0); i++)
            {
                for (int j = 0;j < parkingLot.GetLength(1); j++)
                {
                    Console.Write(parkingLot[i, j] + ",");
                }
                Console.WriteLine();
            }
        }

    }
}
```