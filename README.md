# Interface

## Aim:
To write a C# program using interface concept


## Algorithm:
## step 1:
Create an interface.

## step 2:
Create a child class.

## step 3:
Declare 2 functions deposit() and withdrawal() as abstract methods in the interface.

## step 4:
Create those 2 functions in the child class and perform respective operation.

## step 5:
Use while loop and and switch case to Get the choice from the user whether to perform withdrawal or deposit operation.

## step 6:
After performing the functions display the remaining balance of the user.

## Program:
```
using System;
public interface Bank
{
    void deposit();
    void withdrawal();
}
public class Example : Bank
{
    int amount, ch, balance = 5000;
    public Example()
    {
        Console.WriteLine("1.Deposit\n2.Withdrawal");
        ch = Convert.ToInt32(Console.ReadLine());
        if (ch == 1)
        {
            deposit();
        }
        else
        {
            Console.Write("Enter the amount to withdraw  ");
            withdrawal();
        }
    }
    public void withdrawal()
    {
        int amount = Convert.ToInt32(Console.ReadLine());
        balance -= amount;
        Console.WriteLine("Balance = " + balance);
    }
    public void deposit()
    {
        int amount = Convert.ToInt32(Console.ReadLine());
        balance += amount;
        Console.WriteLine(balance);
    }
}
public class hi
{
    public static void Main()
    {
        Example c = new Example();
        c.deposit();
        c.withdrawal();
    }
}
```


## Output:
![image](https://github.com/Rakshithadevi/Interface/assets/94165326/ad72a2ec-2fbe-4472-98c2-34f0412ed9f2)



## Result:
Thus the C# program using interface concept has been implemented successfully
