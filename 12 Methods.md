# Methods in C#

### ***Methods / Functions***
They are used to divide and sort Functionalities within a class so that the code will be readable even if its long.


#### ***CREATING Methods***
    modifiers returntype methodName()
    {
        // Do anything here.
    }

###### ***Example***
```csharp
static void sayHello()
{
    Console.WriteLine("Hello!");
}
```

#### ***CALLING Methods***
    static void Main(string[] args)
    {
        methodName();
    }

###### ***Example***
```csharp
static void Main(string[] args)
{
    sayHello();
}

static void sayHello()
{
    Console.WriteLine("Hello!");
}
```

    Hello!

___

### ***Comments***
```csharp
// This is a single-line comment.

/* This is a multi-line comment
    You can comment here too! */
```

### ***VARIABLE Scoping***

#### ***Global Variables***
Are **variables declared within** a **class**, it can be accessed within a whole class.

#### ***Local Variables***
Are **variables declared inside** a **method, conditions, loops** and **any other block of code**, it can only be **accessible within** that **block of code**.

___
```csharp
class Program
{
    //GLOBAL Variables

    static string name = "Kkuru";
    static int age = 21;

    static void Main(string[] args)
    {
        introduce();
    }

    static void introduce()
    {
        // LOCAL Variables

        string name = "Ssamu";
        int age = 18;

        Console.WriteLine($"Hi, my name is {name}.");
        Console.WriteLine($"My age is {age}.");
    }
}
```

### ***Parameters / Arguments***
A **value** that needs to be **passed** on a **Method** so that the **method** can use the **value** and **perform various operations** on it.

You can hane as many Arguments / Parameters as you want. They act as a Local Variable inside a method / function.

    modifiers returntype methodName(parameters)
    {
        // Do Anything Here
    }

###### ***Example***

```csharp
static void Main(string[] args)
{
    say("Kkuru")
    say("Ssamu")
}

static void say(string word)
{
    Console.WriteLine(word);
}
```
    Kkuru
    Ssamu


### ***RETURN Keyword***
Used to **return** a **value** from the method. It is used when a method has a result.

Example:  
A method that performs Math Equations.  
A method that Concatenates Strings.

### ***RETURN Type***
The **type** of the **value** that will be **returned, return type** are the same as **datatypes**.

**void** returns **nothing**.  
**int** returns **integers**.  
**string** returns **strings**.  
and so on...

### ***Methods with RETURNS***
    modifiers returntype methodName(arguments)
    {
        // Do anything here
        return value;
    }

___

###### ***Example***
```csharp
static void Main(string[] args)
{
    int x = add(5, 19);
    Console.WriteLine(x)
}

static int add(int num1, int num2)
{
    int sum = num1 + num2;
    return sum
}
```
    24
___

### ***OVERLOADING Methods***
you can use the same method name but different parameters so that you can cater every possibility of a method.

```csharp
static void Main(string[] args)
{
    Console.WriteLine(add(5,19));
    Console.WriteLine(add(5,19,2));
    Console.WriteLine(add(1.25f, 9.15f));
}

static int add(int num1, int num2)
{
    int sum = num1 + num2;
    return sum
}

static int add(int num1, int num2, num3)
{
    int sum = num1 + num2 + num3;
    return sum
}

static float add(float num1, float num2)
{
    float sum = num1 + num2;
    return sum
}
```
    24
    26
    10.4

