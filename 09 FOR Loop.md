# FOR Loop in C#

### ***For Loop***
It is used when you want a Code Block to run repeatedly **WHILE** the **Condition is Met.**  
Its a **more compact format** but **more complicated** version of a **WHILE loop**. **FOR Loops** are commonly used to **iterate** through **Collections** and **Arrays**.

```csharp
for(int i = 0; i < 5; i++)
{
    Console.WriteLine(i);
}
```

    0
    1
    2
    3
    4

### ***ITERATING Arrays***
It means to read every element inside an array and do something with it.

```csharp
string[] names = {"Kkuru","Jin","Jiro","Sana","Mina"};

for(int i; i < 5; i++)
{
    Console.WriteLine(names[i]);
}
```


    Kkuru
    Jin
    Jiro
    Sana
    Mina


### ***Array LENGTH***
You can find out the size of an array by calling their length variable (built-in variable in an array).

```csharp
string[] names = {"Kkuru","Jin","Jiro","Sana","Mina","IU","Ssamu"};

for (int i = 0; i < names.Length; i++)
{
    Console.WriteLine(names[i]);
}
```

    Kkuru
    Jin
    Jiro
    Sana
    Mina
    IU
    Ssamu

*Other Example*

```csharp
string[] names = {"Kkuru","Jin","Jiro","Sana","Mina","IU","Ssamu"};

for (int i = names.Length - 1; i >= 0; i--)
{
    Console.WriteLine(names[i]);
}
```

    Ssamu
    IU
    Mina
    Sana
    Jiro
    Jin
    Kkuru


### ***BREAK Keyword***
Used to **BREAK Out** of a **LOOP** statement **earlier** than it is **expected** to end.

### ***CONDITIONS in For Loop***
You can use Conditions inside a for loop for different reasons like, searching inside an array.

```csharp
string[] names = {"Kkuru","Jin","Jiro","Sana","Mina"};

for(int i = 0; i < names.Length; i++)
{
    if (names[i].Equals("Sana"))
    {
        Console.WriteLine($"We found {names[i]}");
        break;
    }
    else
    {
        Console.WriteLine(names[i]);
    }
}
```

    Kkuru
    Jin
    Jiro
    We found Sana