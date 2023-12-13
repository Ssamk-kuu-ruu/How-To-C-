# Datatype Conversion in C#

## ***Data type Conversion***
It is an act of converting one datatype to another.

### ***Type Casting***
Assigning a value of one datatype to another datatype.

#### ***Implicit Casting***
Converting a smaller type to a larger type size. This is done automatically.

    char -> int -> long -> float -> double

```csharp
int myInt = 10;
double myDouble = myInt;

char myChar = 'B';
int asciiCode = myChar;
```

#### ***Explicit Casting***
Converting a larger type to a smaller size type. It is done manually by using the parentheses with the datatype in it.

    double -> float -> long -> int -> char

```csharp
double myDouble = 236.75;
int x = (int) myDouble;
```

### ***Conversion Method***
It uses a built-in method to convert datatypes from one type to another especially strings.

| | |
| ----------- | ----------- |
| **Convert.ToInt32()** | *string* to *int* | 
| **Convert.ToInt64()** | *string* to *long* |
| **Convert.ToSingle()** | *string* to *float* |
| **Convert.ToDouble()** | *string* to *double* |
| **Convert.ToString()** | *any data type* to *string* |
