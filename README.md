# .NET
My Journey To Becoming a .NET and C# Developer
C# is an object-oriebted programming language for building enterprise apps that run on the .NET framework by Microsoft.
Applications written in C# uses the .NET Framework and its compenents which consist of Common Language Runtime (CLR) and the .NET Framework class library.
CLR manages code at execution time, providing core services such as memory management, code accuracy, and many other aspects of your code. while the class library is a collection of classes, interfaces, and value types that enable you to accomplish a range of common programming tasks, such as data collection, file access, and working with text.

//VARIABLES IN C#
Variables are use for storing values/information which reserves memory location.
Variablea are declared by specifying the name and data type
name are identfiers and can contain letters,numbers and _
name must start with letter or _ and should be descriptive

/VARIABLE TYPES
A data type defines the information that can be stored in a variable, the size of needed memory and the operations that can be performed with the variable.
A line of code that completes an action is called a statement. Each statement in C# must end with a semicolon.

/DECLARING A VARIABLE
int aNumber = 23;
or
in aNumber;
aNumber = 23;

/C# Built-in Data Types
int - integer.
float - floating point number.
double - double-precision version of float.
char - a single character. values assigned using single quotes.
bool - Boolean that can have only one of two values: True or False.
string - a sequence of characters. assigned using double quotes

//RUNNING C# ON COMPUTER
Install integrated development environment (IDE)
Install Visual Studio (VS), choose the default configuration, click File->New->Project and then choose Console Application 

//WRITING FIRST PROGRAM
using System;
namespace MyLearning
{
  class Program{
    static void Main(string[] args){
     Console.WriteLine("Hi"); //print Hi to the console
     int x = 4;
     double y = 8;
     Console.WriteLine(x);
     Console.WriteLine("x : {0}, y : {1}", x, y);
    }
  }
}
//Every console application in C# should contain Main method
To run your pragrm in VS, press Ctrl+F5
Console uses a text-only code.



