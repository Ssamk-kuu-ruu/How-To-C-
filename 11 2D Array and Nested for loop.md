# 2D Array and Nested For Loops in C#

### ***2D Array***
It's **arrays within** an **array**, it basically looks like a table with rows and columns.

Like **1D Arrays**, it can only store **one datatype** at a time.

### ***Declaring 2D Arrays***
#### ***Declare with values***

    datatype[,] identifiers = {  
        {val1, val2},
        {val1, val2},
        {val1, val2}
    };
___
###### ***Example***

```csharp
string[,] users =
{
    {"Kkuru", "Kkuru123"},
    {"Jiro", "Jiro123"},
    {"Jin", "Jin123"},
    {"Ssamu", "Ssamu123"},
    {"Wonchae", "Wonchae123"}
};
```
#### ***Declaring without values***

    datatype[,] identifiers = new datatype [rows, cols];

___
###### ***Example***
```csharp
string[,] users = new string [4, 2];
```

### ***Accessing 2D Arrays***

```csharp
string[,] users =
{
    {"Kkuru", "Kkuru123"},
    {"Jiro", "Jiro123"},
    {"Jin", "Jin123"},
    {"Ssamu", "Ssamu123"},
    {"Wonchae", "Wonchae123"}
};
```
| INDEX | 0 | 1 
| ----------- | ----------- | -----------
| 0 | "Kkuru" **[0,0]** | "Kkuru123" **[0,1]**
| 1 | "Jiro" **[1,0]** | "Jiro123" **[1,1]**
| 2 | "Jin" **[2,0]** | "Jin123" **[2,1]**
| 3 | "Ssamu" **[3,0]** | "Ssamu123" **[3,1]**
| 4 | "Wonchae" **[4,0]** | "Wonchae123" **[4,1]**

___

#### ***Read Values***

    Console.WriteLine(identifier[row,col]);

___
###### ***Example***
```csharp
Console.WriteLine(users[0,1]);
```
___

#### ***Write Values***
    identifier[row,col] = value;
___
###### ***Example***
```csharp
users[0,0] = "Aeri";
```
___



### ***NESTED FOR Loop***
it is a **for loop** inside a **for loop**.

```csharp
for(int i = 0; i < 5; i++)
{
    Console.WriteLine("Loop " + i);

    for(int x = 0; x > 5; x++)
    {
        Console.WriteLine(x);
    }
    Console.WriteLine();
}
```
    Loop 0
    0
    1
    2
    3
    4

    Loop 1
    0
    1
    2
    3
    4

    Loop 2
    0
    1
    2
    3
    4

    Loop 3
    0
    1
    2
    3
    4

    Loop 4
    0
    1
    2
    3
    4

___

### ***Iterating 2D Arrays using Nested FOR Loops***
We can use Nested For Loops or For Each Loops to iterate through 2D Array.

```csharp
string[,] users =
{
    {"Kkuru", "Kkuru123"},
    {"Jiro", "Jiro123"},
    {"Jin", "Jin123"},
    {"Ssamu", "Ssamu123"},
    {"Wonchae", "Wonchae123"}
};

for(int row = 0; row < users.GetLength[0]; row++)
{
    for(int col = 0; col < users.GetLength[1]; col++)
    {
        Console.WriteLine(users[row,col]);
    }

    Console.WriteLine();
}
```
    Kkuru
    Kkuru123

    Jiro
    Jiro123

    Jin
    Jin123

    Ssamu
    Ssamu123

    Wonchae
    Wonchae123

___

### ***Iterating 2D Arrays using For-Each Loop***

```csharp
string[,] users =
{
    {"Kkuru", "Kkuru123"},
    {"Jiro", "Jiro123"},
    {"Jin", "Jin123"},
    {"Ssamu", "Ssamu123"},
    {"Wonchae", "Wonchae123"}
};

int i = 1;

foreach(string info in users)
{
    Console.WriteLine(info);
    if (i % 2 == 0)
    {
        Console.WriteLine();
        i++;
    }
}
```
    Kkuru
    Kkuru123

    Jiro
    Jiro123

    Jin
    Jin123

    Ssamu
    Ssamu123

    Wonchae
    Wonchae123