# Overloaded Constructors
```cs
namespace LearningCsharp
{
    class Program
    {
        public static void Main(string[] args)
        {
            Pizza pizza1 = new Pizza("stuffed crust", "red sauce", "mozzarella", "pepperoni");
            Pizza pizza2 = new Pizza("stuffed crust", "red sauce", "mozzarella");
            Pizza pizza3 = new Pizza("stuffed crust", "red sauce");
            Pizza pizza4 = new Pizza("stuffed crust");
            Pizza pizza5 = new Pizza();
        }

        class Pizza
        {
            String bread;
            String sauce;
            String cheese;
            String topping;
            public Pizza(string bread, string sauce, string cheese, string topping)
            {
                this.bread = bread;
                this.sauce = sauce;
                this.cheese = cheese;
                this.topping = topping;
            }
            public Pizza(string bread, string sauce, string cheese)
            {
                this.bread = bread;
                this.sauce = sauce;
                this.cheese = cheese;
            }
            public Pizza(string bread, string sauce)
            {
                this.bread = bread;
                this.sauce = sauce;            
            }
            public Pizza(string bread)
            {
                this.bread = bread;
            }
            public Pizza()
            {
            }
        }



    }
}
```