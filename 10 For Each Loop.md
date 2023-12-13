# FOR EACH Loop in C#

### ***For Each Loop***
Used to iterate through collections like arrays easily without knowing the size of the collection.

### ***Iterating Arrays***
It means to read every element inside an array and do something with it.

```csharp
string[] names = {"Kkuru", "Jiro", "Jin","Ssamu", "Wonchae"};

foreach(string name in names)
{
    Console.WriteLine(name);
}
```
    Kkuru
    Jiro
    Jin
    Ssamu
    Wonchae

### ***Break Keyword***
Used to **BREAK Out** of a **LOOP** statemant **earlier** than it is **expected** to end.

```csharp
string[] names = {"Kkuru", "Jiro", "Jin", "Ssamu", "Wonchae"};

foreach(string name in names)
{
    Console.WriteLine(name);
    break;
}
```

    Kkuru

### ***Conditions in FOR-EACH Loop***
You can use Conditions inside a for-each loop for different reasons like, searching inside an array.

```csharp
string[] names = {"Kkuru", "Jiro", "Jin", "Ssamu", "Wonchae"};

foreach(string name in names)
{
    if (name = "Jin")
    {
        Console.WriteLine($"I found {name}");
        break;
    }
}
```
    Kkuru
    Jiro
    I found Jin