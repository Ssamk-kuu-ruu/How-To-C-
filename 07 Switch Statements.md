# Switch Statements in C#

### ***Switch Statements***
it is a similar to a Conditional Statement but only checks for equality and only works with **strings**, **char**, **int**, and **enums**.

```csharp
char grades = 'A';

switch(grades)
{
    case 'A':
        Console.WriteLine("Outstanding!");
        break;
        
    case 'B':
        Console.WriteLine("Excellent!");
        break;

    case 'C':
        Console.WriteLine("Satisfactory");
        break;
        
    case 'D':
        Console.WriteLine("Good");
        break;

    case 'E':
        Console.WriteLine("Needs Improvement");
        break;

    case 'F':
        Console.WriteLine("Failed");
        break;

```

### ***Case Keyword***
Used to define a "*Case*" in switch statement.

### ***Default Keyword***
Often used to **handle values** that are **NOT** on the **Case**. It is recommended that this keyword is used on the **END** of a **switch statement**.

```csharp
    default:
        Console.WriteLine("Invalid Grade");
        break;
}
```

### ***Break Keyword***
used to **Break Out** of a **switch statement** or **loop statements** without executing the whole block of code inside it.