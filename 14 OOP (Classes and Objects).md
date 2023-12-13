# Classes and Objects in C#

## ***Object - Oriented Programming***
It focuses on implementing real world objects using **Classes** to create variation of **Objects**, that has attributes and purpose.

It helps us create much **flexible** and **efficient** code than **procedural programming**.

## ***Classes***
It is **created** by the programmer, it will act as a **blueprint** of an **object** that you want to **implement** in your **program**.

They **contain** all the **attributes** and **methods** that your desired **object** should have.

## ***Objects***
It is **created** by instantiating a **Class**.

It is anything that has an **attribute** and a **purpose.**

## ***Attributes***
These are the **global variables** declared inside the **class** of our **object**.

it is used to **create variations** of an **object** using only one class.

---

### ***CLASS Creation***
**Person**
- First Name
- Last Name
- Sex
- Age

```csharp
public Person class{
    // Attributes
    public string firstName;
    public string lastName;
    public char sex;
    public int age;

    // Methods or Purpose
}
```
---

### ***CLASS Instantiation***
The process of creating an **Object** using a **class** so we can use it on our program.

```csharp
Person p1 = new Person();
Person p2 = new Person();
Person p3 = new Person();
```
---

### ***ACCESSING Attributes***

#### ***WRITING Attributes***
    identifier.attribute = value;

#### ***READING Attributes***
    Console.WriteLine(identifier.attribute);

---
```csharp
p1.firstName = "Kkuru";
p1.lastName = "Lee";
p1.sex = 'M';
p1.age = 18;

p2.firstName = "Jiro";
p2.lastName = "Pasco";
p2.sex = 'M';
p2.age = 21;

p3.firstName = "Wonchae";
p3.lastName = "Aeri";
p3.sex = 'F';
p3.age = 25;


Console.WriteLine(p1.firstName + " " + p1.lastName);
Console.WriteLine(p2.firstName + " " + p2.lastName);
Console.WriteLine(p3.firstName + " " + p3.lastName);
```