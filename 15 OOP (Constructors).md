# Constructors in C#

### ***Constructors***
Is a **method** called when you **instantiate a class / create an object**.

It is used to **initialized** the **attributes** of an **object** or **run** a **block of code** when an **object is created**.

### ***CREATING Constructors***
**Constructor method** are **named** after their **Class Name**.

    modifiers className class{
        modifiers className(){
            //Constructor
        }
    }

```csharp
class Product
{
    public Product()
    {
        Console.WriteLine("Product Created!")
    }
}
```
---

### ***THIS keyword***
The **this** keyword refers to the **class** itself.

The **this keyword** will **enables** you to **access global variables** inside the **class** if you have the **same variable names** in a **parameter**.

```csharp
class Product
{
    public string name;
    public float price;

    public Product(string name, float price)
    {
        this.name = name;
        this.price = price;
    }
}

class Program
{
    static void Main(string[] args)
    {
        Product p1 = new Product("Milk", 150);
        Product p2 = new Product("Coke", 75);
        Product p3 = new Product("Bread", 25);
    }
}
```