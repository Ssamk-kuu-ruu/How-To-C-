# Inheritance in C#

### ***Inheritance***
An **OOP technique** used to **inherit attributes, properties,** and **methods** from one **class** to **another**.

### ***Base Class***
The class where we will inherit the attributes and methods.

### ***Derived Class***
The class who will inherit attributes annd methods from a base class.

### ***USING Inheritance***
**':' after Derived Class Name**

    modifiers class derivedClassName: baseClassName{
        // Attributes and Methods
    }

```csharp
class Program
{
    static void Main(string[] args)
    {
        Person p = new Person();
        p.name = "Kkuru";
        p.sex = "Male";
        p.age = 21;
        p.introduceSelf();

        Toddler t = new Toddler();
        t.name = "Wonchae";
        t.sex = "Female";
        t.age = 1;
        t.introduceSelf();
        t.cry();
    }
}

class Person
{
    public string name 
    {
        get;
        set;
    }

    public string sex
    {
        get;
        set;
    }

    public int age
    {
        get;
        set;
    }

    public void introduceSelf()
    {
        Console.WriteLine("Name : " + name);
        Console.WriteLine("Sex  : " + sex);
        Console.WriteLine("Age  : " + age);

    }
}

class Toddler : Person
{
    public void cry()
    {
        Console.WriteLine(name + " is crying.");
    }
}
```

### ***OVERRIDING Constructors***
**You are required to call the constructor of the superclass**

### ***BASE Keyword***
can only be used by **derived class** and it is **used** to **call** their **base class** so we can access their constructions, attributes, and methods.

```csharp
class Program
{
    Person p = new Person("Kkuru", "Male", 21);
    p.introduceSelf();

    Toddler t = new Toddler("Wonchae", "Female", 1, "Peek-a-Boo");
    t.faveGame();
    t.introduceSelf();
    t.cry();

    Child c = new Child("Ssamu", "Female", 5, "Valorant", "Sleeping");
    c.introduceSelf();
    c.cry();
    c.doHobby();
}

class Person
{
    public string name 
    {
        get;
        set;
    }

    public string sex
    {
        get;
        set;
    }

    public int age
    {
        get;
        set;
    }

    public Person(string name, string sex, int age)
    {
        this.name = name;
        this.sex = sex;
        this.age = age;
    }

    public void introduceSelf()
    {
        Console.WriteLine("Name : " + name);
        Console.WriteLine("Sex  : " + sex);
        Console.WriteLine("Age  : " + age);

    }
}

class Toddler : Person
{
    public string faveGame
    {
        get;
        set;
    }

    public Toddler(string name, string sex, int age, string faveGame) : base(name, sex, age)
    {
        this.faveGame = faveGame;
    }

    public void cry()
    {
        Console.WriteLine(name + " is crying.");
    }
}

class Child : Toddler
{
    public string hobby
    {
        get;
        set;
    }

    public Child(string name, string sex, int age, string faveGame, string hobby) : base(name, sex, age, faveGame)
    {
        this.hobby = hobby;
    }

    public void doHobby()
    {
        Console.WriteLine(name + " is " + hobby);
    }
}
```

### ***OVERRIDING Methods***
**To retain the Functionality from the Base Class use the Base Keyword to call the Method**

```csharp
class Program
{
    Person p = new Person("Kkuru", "Male", 21);
    Toddler t = new Toddler("Wonchae", "Female", 1, "Peek-a-Boo");
}

class Person
{
    public string name 
    {
        get;
        set;
    }

    public string sex
    {
        get;
        set;
    }

    public int age
    {
        get;
        set;
    }

    public Person(string name, string sex, int age)
    {
        this.name = name;
        this.sex = sex;
        this.age = age;
    }
}

class Toddler : Person
{
    public string faveGame
    {
        get;
        set;
    }

    public Toddler(string name, string sex, int age, string faveGame) : base(name, sex, age)
    {
        this.faveGame = faveGame;
    }
}
```