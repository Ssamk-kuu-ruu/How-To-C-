# Variables and Data Types in C#

### ***Variables***
Variables are used to **store** up **temporary data** to be used in our **program's runtime**.

### ***Data Types***
The **Type** of **Data** inside our variable.

|  |  |  |
| ----------- | ----------- | ----------- |
| **Characters** | *char* | Holds a Single Character
| **String** | *string* | Holds a Set of Characters/ Texts
| **Boolean** | *bool* | Holds True of False
| **Integers** | *int* | -2147483648 to 214748348
|  | *long* | -9223372036854775808 to 9223372036854775808
| **Floating Point** | *float* | 6/7 decimals
|  | *double* | 15 decimals

### ***Identifiers***
It is the **Name** of the **Variable** that the **programmer indicated** it is **used** to **read** and **write** inside the **variable**.

#### Rules of Identifiers
- You cannot use any special characters other than underscore (-)
- You cannot use whitespaces
- You cannot use numbers alone
- You cannot use numbers to be the first character of the identifier
- You cannot use numbers but with letters

### ***Declaring Variables***
#### **Syntax:** 
***datatype*** identifier;  
***datatype*** identifier = value;  
***datatype*** identifier1, identifier2;  
***datatype*** identifier1 = value, identifier2 = value;

```csharp
string name = Kkuru;
int age = 21;
char sex = 'M'      // single quote if char
bool isTall = true; // case sensitive
float ave = 1.5f;   // 'f' to indicate float
```

### ***Reassigning Variables***
#### **Syntax:**
identifier = value;

```csharp
string name;
int age;

name = "Kkuru";
age = 21;
```

### ***Console.WriteLine()***
1. Used to display something in the console.
2. We can display a variable's value by indicating its identifier inside the parentheses.

```csharp
int age = 21;
Console.WriteLne(age);
```

### ***Concatenation***
The process of joining Strings together with the plus operator. You can concatenate **INSIDE** a **Variable** or on the **WriteLine Statement**.


| Concatenation  | Not Concatenation |
| ----------- | ----------- |
| "Hello" + "World" | 2 + 3 |
| "2" + "3" | 'a' + 3 |
| 'a' + "b" |  |
| 2 + "3" |  |
