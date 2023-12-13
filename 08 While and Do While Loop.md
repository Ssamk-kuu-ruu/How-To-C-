# While and Do While Loop in C#

### ***WHILE Loop***
It is used when you want a Code Block to run repeatedly **WHILE** a **CONDITION** is met.

```csharp
int 0;

while (i < 5)
{
    Console.WriteLine(i);
    i++;
}
```

#
    0
    1
    2
    3
    4

### ***ITERATING Arrays***
It means, reads every element inside an array and do something with it.

```csharp
int i = 0;
string[] names = {"Kkuru", "Jin", "Jiro", "Sana", "Mina"};

while (i < 5)
{
    Console.WriteLine(names[i]);
    i++;
}
```

#
    Kkuru
    Jin
    Jiro
    Sana
    Mina

### ***Array LENGTH***
You can find out the size of an array by calling their length variable(built in variable in an array)

```csharp
int i = 0;
string[] names = {"Kkuru", "Jin", "Jiro", "Sana", "Mina"};
    
while(i <= names.length);
{
    Console.WriteLine(names[i]);
    i++;
}
```
#
    Kkuru
    Jin
    Jiro
    Sana
    Mina


### ***DO - WHILE Loop***
Same as the While Loop but it **EXECUTES** the Code Block first before checking the **CONDITION**.

```csharp
int j = 0;

do
{
    Console.WriteLine(j);
    j++;
}
while (j < 5);
```
#
    0
    1
    2
    3
    4

### ***BREAK Keyword***
Used to **BREAK Out** of a **LOOP** Statement **earlier** than it is **expected** to end.

```csharp
int i = 0;

string[] names = {"Kkuru", "Jin", "Jiro", "Sana", "Mina"};

while (i < 5)
{
    Console.WriteLine(names[i]);
    i++;
    break;
}
```
#
    Kkuru

### ***Conditions in WHILE Loop***

You can use Conditions inside a while loop for different reasons like, searching inside an array.

```csharp
string[] names = {"Kkuru", "Jin", "Jiro", "Sana", "Mina"};
int i = 0;

while (i < 5)
{
    if(names[i].Equals("Jiro"))
    {
        Console.WriteLine("We found " + names[i]);
        break;
    }
    else
    {
        Console.WriteLine(names[i]);
    }
    i++;
}
```
#
    Kkuru
    Jin
    Jiro