# Interface
### Aim:
To write a C# program using interface concept.

### Algorithm:
#### Step 1 :
Create an interface.

#### Step 2 :
Create a child class.

 #### Step 3 :
Declare two functions deposit() and withdrawal() in the interface.

#### Step 4 :
Create those two functions in the child class and perform respective operation.

#### Step 5 :
Use if else loop to Get the choice from the user whether to perform withdrawal or deposit operation.

#### Step 6 :
After performing the functions display the remaining balance of the user.

### Program:

                              Developed by : SWATHIKA G
                              Register No : 212221230113
```
using System;
namespace Hello
{
    class Program
    {
        public interface bank
        {
            void deposit(int amount);
            void withdrwal(int amount);
        }
        public class bank1:bank
        {
            int balance = 1000;
            int amount;
            public void deposit(int amount)
            {
                balance = balance+amount;
                Console.WriteLine(balance);
            }
            public void withdrwal(int amount)
            {
                balance = balance-amount;
                Console.WriteLine(balance);
            }
            public static void Main()
            {
                bank1 obj = new bank1();
                Console.WriteLine("Enter your choice :");
                Console.WriteLine("Enter 1 to deposit");
                Console.WriteLine("Enter 2 to withdraw");
                int ch = Convert.ToInt32(Console.ReadLine());
                if (ch == 1)
                {
                    Console.WriteLine("Enter the amount to be deposited:");
                    int amount = Convert.ToInt32(Console.ReadLine());
                    Console.WriteLine("Balance Amount in your Account : ");
                    obj.deposit(amount);
                }
                else if (ch == 2)
                {
                    Console.WriteLine("Enter the amount to be withdrawed:");
                    int amount = Convert.ToInt32(Console.ReadLine());
                    Console.WriteLine("Balance Aamount in your Account : ");
                    obj.withdrwal(amount);
                }
            }
        }

    }
}

```
### Output:
![OP](https://raw.githubusercontent.com/SOWMIYA2003/Interface/main/aa1.png)
![OP](https://raw.githubusercontent.com/SOWMIYA2003/Interface/main/aa12.png)

### Result:
Thus a C# program using interface concept is written and executed successfully.
