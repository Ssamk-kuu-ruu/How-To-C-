# Encapsulation in C#

### ***Encapsulation***
An **OOP** technique used to **hide** data from direct access.

### ***Encapsulation Advantages***
1. It **hides direct access** to our **variables**, it also **hides** our **implementation** of how we **get** and **set** a certain value.
2. We can **decide** whether we want to **make** a **variable read - only** or **write - only**.

### ***USING Encapsulation***
**Declare Attributes** as **PRIVATE**.

    modifiers className class{

        //Private Attributes

    }

```csharp
class User
{
    //private fields
    private int userID;
    private string userName;
    private string firstName, lastName;
}
```

---

### ***Getter and Setters***
Used to **get** and **set** encapsulated variables.

    //field
    private int userID;

    //property
    public int UserID{
        get{
            return userID;
        }
        set{
            userID = value;
        }
    }

```csharp
class User
{
    //private fields
    private int userID;
    private string userName;
    private string firstName, lastName;

    //properties
    public int UserID
    {
        get {return userID;}
        set
        { 
            if (value >=1000) userID = value;
            else Console.WriteLine("Error, User ID must not be below 1000.");
        }
    }

    public string UserName
    {
        get{return userName;}
        set{
            userName = value;}
    }

    public string FirstName
    {
        get{return firstName;}
        set{firstName = value;}
    }

    public string LastName
    {
        get{return lastName;}
        set{lastName = value;}
    }

    public string FullName
    {
        get{return firstName + " " + lastName;}
    }
    
    public User(int userID, string userName, string firstName, string lastName)
    {
        UserID = userID;
        UserName = userName;
        Firstname = firstName;
        LastName = lastName;
    }
}
```
---

### ***USING Getter and Setter***

```csharp
class Program
{
    static void Main(string[] args)
    {
        User user = new User(202080094, "HelloWorld","Kkuru", "Lee");

        Console.WriteLine(user.FullName);
        // Kkuru Lee
    }
}
```

--- 

### ***Getter and Setter (shortcut)***

    // Automatic Property
    public int userID{
        get;
        set;
    }

```csharp
class User
{
    // Automatic Properties
    public int userID
    {
        get;
        set;
    }

    public string userName
    {
        get;
        set;
    }

    public string firstName
    {
        get;
        set;
    }

    public string lastName
    {
        get;
        set;
    }

    public User(int userID, string userName, string firstname, string lastname)
    {
        this.userID = userID;
        this.userName = userName;
        this.firstName = firstName;
        this.lastName = lastName;
    }
}

class Program
{
    static void Main(string[] args)
    {
        User user = new User(202080094, "HelloWorld", "Kkuru", "Lee");

        user.firstName = "Jiro";
    }
}
```