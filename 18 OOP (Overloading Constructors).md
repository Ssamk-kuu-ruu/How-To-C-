# Overloading Constructors in C#

### ***OVERLOADING Constructors***
An **OOP** technique used to **create** multiple constructors with different arguments. It is used to cope up with the needs of a certain instance of an object.

*Same as Method Overloading*

**Create Multiple Constructoes with Different Arguments**


    modifiers class className{
        // Declare Attributes Here
        className(arguments){

        }

        className(arguments){

        }
    }

```csharp
class Product
{
    public int productID
    {
        get;
        set;
    }

    public string productName
    {
        get;
        set;
    }

    public string productDescription
    {
        get;
        set;
    }

    public int productStock
    {
        get;
        set;
    }

    public int productPrice
    {
        get;
        set;
    }

    public Product(int productID, string productName, string productDescription, int productStock, int productPrice)
    {
        this.productID = productID;
        this.productName = productName;
        this.productDescription = productDescription;
        this.productStock = productStock;
        this.productPrice = productPrice;
    }

    public Product(int productID, string productName, int productStock, int productPrice)
    {
        this.productID = productID;
        this.productName = productName;
        this.productStock = productStock;
        this.productPrice = productPrice;
    }
}

class Program
{
    static void Main(string[] args)
    {
        Product p = new Product(1, "Milk", 5, 150);
        Product p1 = new Product(2, "Coffee", "to make you awake", 5, 100)
    }
}
```