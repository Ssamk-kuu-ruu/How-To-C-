# Conditionals in C#

### ***Conditional Statements***
Allows a program to make action based on the*given condition*. It makes our program smarter. Typically it *compares two values* so that our program can decide what action should be taken.

| Label | Symbol | Syntax |
| ----------- | ----------- | ----------- |
| Equals | == | x == y
| NOT Equals | != | x != y
| Less Than | < | x < y
| Less Than or Equals | <= | x<= y
| Greater Than | > | x > y
| Greater Than or Equals | >= | x >= y

### **IF Statement**
Handles **1 Conditional Expression**, it **either** does **SOMETHING** or **NOTHING**.

```csharp
int age = 18;

if(age >= 18){
    Console.WriteLine("You can drive.")
}
```

### **IF-ELSE Statement**
Handles **2 Conditional Expressions**, it **either** does the first Code Block or the second Code Block.

```csharp
Console.Write("Population: ");

int currentPopulation = ConvertToInt32(Console.ReadLine());
int maxPopulation = 100;

if (currentPopulation == maxPopulation)
{
    Console.WriteLine("Population Stable.");
}
else
{
    Console.WriteLine("Overpopulated.");
}
```

### **IF - ELSE IF - ELSE**
Handles **3 or More Conditional Expressions**, The possibility of this Statements are limitless it will run a certain code block based on the condition.

```csharp
Console.Write("Age: ");
int age = Convert.ToInt32(Console.ReadLine);

if (age >= 24)
{
    Console.WriteLine("Adult");
}
else if (age >= 18)
{
    Console.WriteLine("Young Adult");
}
else if (age >= 13)
{
    Console.WriteLine("Teenager");
}
else if (age >= 4)
{
    Console.WriteLine("Kid");
}
else
{
    Console.WriteLine("Baby");
}
```

### **Nested Conditional Statement**
A **Conditional Statement** within a **Conditional Statement**. It can be an any type of **Conditional Statement**.

```csharp
int age = 18;
bool isRegistered = true;

if (age >= 18)
{
    if (isRegistered)
    {
        Console.WriteLine("You can vote!");
    }
    else
    {
        Console.WriteLine("You can register as a Voter!");
    }
}

else
{
    Console.WriteLine("Access Denied!");
}
```


### **Equals Method**

```csharp
Console.Write("Password: ");
string pword = Console.ReadLine();

if(pword.Equals("imcute123"))
{
    Console.WriteLine("Login Successul!");
}
else
{
    Console.WriteLine("Access Denied!");
}
```

### **Equals Method (*Ignoring Case*)**

```csharp
Console.Write("Username: ");
string user = Console.Readline();

if(user.Equals("kkuru",StringComparison.InvariantCultureIgnoreCase))
{
    Console.WriteLine("User Exist.");
}
else
{
    Console.WriteLine("User Not Found.");
}
```

## ***Logical Operators***

| Label | Symbol | Syntax | Description
| ----------- | ----------- | ----------- |----------- |
| AND | && | condition && condition | Both Conditions need to be True.
| OR | \|\| | condition \|\| condition | Either Conditions need to be True.
| NOT | ! | !condition | Inverts the Current Condition

#### *NOT*
```csharp
int age = 18;

if(!(age >= 18))
{
    Console.WriteLine("Access Denied!");
}
else
{
    Console.WriteLine("Access Granted!");
}
```

#### *AND*
```csharp
int age = 12;
bool isRegistered = true;

if (age >= 18 && isRegistered)
{
    Console.WriteLine("You can vote");
}
else
{
    Console.WriteLine("Access Denied!");
}
```
#### *OR*
```csharp
bool level = 50;
bool isVIP = true;

if(level >= 100 || isVIP)
{
    Console.WriteLine("You have obtained the legendary item!");
}
else
{
    Console.WriteLine("You don't meet the requirements");
}
```