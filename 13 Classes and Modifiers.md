# Classes and Modifiers in C#

### ***Classes***
It is **created** by the programmer, it will act as a **blueprint** of an **object** that you want to **implement** in your **program**.

They **contain** all the **attributes** and **methods** that your desired **object** should have.

### ***CREATING Classes***
We can create classes inside our current file or create another file in the solution explorer.

```csharp 

class Arithmetic
{
    public int add(int num1, int num2)
    {
        return num1 + num2;
    }

    public int subtract(int num1, int num2)
    {
        return num1 - num2;
    }

    public int multiply(int num1, int num2)
    {
        return num1 * num2;
    }

    public int divide(int num1, int num2)
    {
        retun num1 / num2;
    }
}

```
___

### ***CLASS Instantiation***
The process of creating an **Instance** of a class so we can use it on our program. These can also be called **objects**.

    ClassName identifier = new ClassName();

###### ***Example***

```csharp

Arithmetic a = new Arithmetic();

a.add(5,2);

```
___

### ***ACCESS Modifiers***
Used to modify where classes, variables, and methods are accessible.

| Modifier | Description |
| ----------- | ----------- |
| default or **private** | It can only be accessed inside its own class. |
| **public** | The class can be accessed in all classes. |
| **internal** | The methods and variables can only be accessed in the same assembly not other assemblies. |
| **protected** | It can only be accessed in the same class or in a class that is inherited from that class |


### ***STATIC***
#### ***classes***
Are classes that cannot be instantiated and it shall only contain static methods and variables.

#### ***methods and variables***
Are methods and variables tat belongs to the class itself and not the instance.

```csharp

class Arithmetic
{
    public static int add(int num1, int num2)
    {
        return num1 + num2;
    }

    public static int subtract(int num1, int num2)
    {
        return num1 - num2;
    }

    public static int multiply(int num1, int num2)
    {
        return num1 * num2;
    }

    public static int divide(int num1, int num2)
    {
        retun num1 / num2;
    }
}

class Program
{
    static void Main(string[] args)
    {
        Arithmetic.add(5,2);
    }
}

```
___

### ***READONLY Keyword***
A keyword used so that a variable cannot be reassigned to a new value.

    public static readonly float PI = 3.14


