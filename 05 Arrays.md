# Arrays in C#

is a Collection of Multiple Values in a **Single  Variable** with the **Same Datatype**. They are governed by using an **index**.

### ***Elements***
The individual values in an array.

## ***Declaring Arrays***
### ***Declare with Values***

```csharp
string[] names = {"Kkuru", "Jiro", "Jin"};
```

### ***Declare without Values***

```csharp
string[] names = new string[4];
```


## ***Index***
A number that represents a position in a collection.

### ***Accessing Array***

| ***Value*** | "Kkuru" | "Jiro" | "Jin" | "Ssamu" | "Mina" |
| ----------- | ----------- | ----------- | ----------- | ----------- | ----------- |
| ***Index*** | 0 | 1 | 2 | 3 | 4 |

### ***Reading Array Element***
```csharp
names[0];
```

### ***Assigning Array Element***
```csharp
names[0] = "Sana";
```

### ***Assigning Array Element with User Input***
```csharp
names[0] = Console.ReadLine();
```