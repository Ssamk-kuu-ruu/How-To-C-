# Object Methods in C#

### ***OBJECT METHODS***
Are **methods** declared inside an **Object Class.**  
**Object Methods** are **considered** as the **Object's purpose.**

### ***CREATING Object Methods***
**Object Methods** are same as the **Methods** that tackled.

    modifiers className class{
        modifiers returntype methodName(arguments){
            // Do anything here;
        }
    }

```csharp
class Character
{
    public string name, dialog;
    public int hp, mp, lvl;

    public Character(string name, string dialog, int hp, int mp, int lvl)
    {
        this.name = name;
        this.dialog = dialog;
        this.hp = hp;
        this.mp = mp;
        this.lvl = lvl;
    }

    public void introduce()
    {
        Console.WriteLine("I am " + name);
    }

    public void sayDialog()
    {
        Console.WriteLine(name + " : " + dialog);
    }

    public void checkStats()
    {
        Console.WriteLine("Name  : " + name);
        Console.WriteLine();
        Console.WriteLine("Level : " + lvl);
        Console.WriteLine("HP    : " + hp);
        Console.WriteLine("MP    : " + mp);
    }
}
```

---

### ***CALLING Object Methods***
**Object Methods** are same as the **Methods** that tackled.

    ClassName cn = new ClassName(constructor);
    cn.methodName(arguments);

```csharp
class Program
{
    static void Main(string[] args)
    {
        Character c = new Character("Kkuru", "Hello World", 100, 50, 1);
        c.introduce;
        // I am Kkuru
        c.sayDialog;
        // Kkuru : Hello World
        c.checkStats;
        /* Name  : Kkuru
        
           Level : 1
           HP    : 100
           MP    : 50
         */
    }
}
```