using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _1
{
    using System;
    using System.Collections.Generic;

    class StockSystem
    {
        static void Main()
        {
            
            Dictionary<string, int> stock = new Dictionary<string, int>();

            
            stock["Rice"] = 50;
            stock["Canned Goods"] = 30;
            stock["Water Bottles"] = 100;

            while (true)
            {
                Console.WriteLine("Stock Management (SDG 12)");
                Console.WriteLine("");
                Console.WriteLine("1. View Stock");
                Console.WriteLine("2. Add Item");
                Console.WriteLine("3. Update Quantity");
                Console.WriteLine("4. Remove Item");
                Console.WriteLine("5. Exit");
                Console.WriteLine("");
                Console.Write("Choose: ");

                int choice = Convert.ToInt32(Console.ReadLine());

                switch (choice)
                {
                    case 1:
                        Console.WriteLine("\nCurrent Stock:");
                        foreach (var item in stock)
                        {
                            Console.WriteLine(item.Key + ": " + item.Value);
                        }
                        break;

                    case 2:
                        Console.Write("Enter item name: ");
                        string newItem = Console.ReadLine();
                        Console.Write("Enter quantity: ");
                        int qty = Convert.ToInt32(Console.ReadLine());
                        stock[newItem] = qty;
                        Console.WriteLine("Item added!");
                        break;

                    case 3:
                        Console.Write("Enter item name to update: ");
                        string updateItem = Console.ReadLine();
                        if (stock.ContainsKey(updateItem))
                        {
                            Console.Write("Enter new quantity: ");
                            stock[updateItem] = Convert.ToInt32(Console.ReadLine());
                            Console.WriteLine("Updated!");
                        }
                        else
                        {
                            Console.WriteLine("Item not found.");
                        }
                        break;

                    case 4:
                        Console.Write("Enter item name to remove: ");
                        string removeItem = Console.ReadLine();
                        if (stock.Remove(removeItem))
                            Console.WriteLine("Removed!");
                        else
                            Console.WriteLine("Item not found.");
                        break;

                    case 5:
                        return;

                    default:
                        Console.WriteLine("Invalid choice.");
                        break;
                }
            }
        }
    }
}
