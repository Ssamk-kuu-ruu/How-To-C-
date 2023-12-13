# User Input in C#

### ***Console.ReadLine()***
Used for inputting a string. 

```csharp
string name;

Console.Write("Name: ");
name = Console.ReadLine();

Console.WriteLine("I am" + name);
```
### ***Console.Read()***
Used for inputting a Character by pressing Enter in the keyboard.

```csharp
char letter;

Console.Write("Letter: ");
letter = (char) Console.Read();

Console.WriteLine(letter);
```
### ***Console.ReadKey()***
Used for inputting a Character by pressing a Letter in the keyboard.

```csharp
char letter;

Console.Write("Press a letter: ");
letter = Console.ReadKey().KeyChar;

Console.WriteLine("\nYou pressed" + letter);
```

It is also used to delay printed *WriteLines*.

```csharp
Console.WriteLine("Hi!");
Console.ReadKey();
Console.WriteLine("I am Kkuru");
Console.ReadKey();
Console.WriteLine("Goodbye!");
```
