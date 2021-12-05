# .NET
My Journey To Becoming a .NET and C# Developer
C# is an object-oriebted programming language for building enterprise apps that run on the .NET framework by Microsoft.
Applications written in C# uses the .NET Framework and its compenents which consist of Common Language Runtime (CLR) and the .NET Framework class library.
CLR manages code at execution time, providing core services such as memory management, code accuracy, and many other aspects of your code. while the class library is a collection of classes, interfaces, and value types that enable you to accomplish a range of common programming tasks, such as data collection, file access, and working with text.

# VARIABLES IN C#
Variables are use for storing values/information which reserves memory location.
Variablea are declared by specifying the name and data type
name are identfiers and can contain letters,numbers and _
name must start with letter or _ and should be descriptive

# VARIABLE TYPES
A data type defines the information that can be stored in a variable, the size of needed memory and the operations that can be performed with the variable.
A line of code that completes an action is called a statement. Each statement in C# must end with a semicolon.

# DECLARING A VARIABLE
int aNumber = 23;
or
in aNumber;
aNumber = 23;

# C# Built-in Data Types
int - integer.
float - floating point number.
double - double-precision version of float.
char - a single character. values assigned using single quotes.
bool - Boolean that can have only one of two values: True or False.
string - a sequence of characters. assigned using double quotes

# RUNNING C# ON COMPUTER
Install integrated development environment (IDE)
Install Visual Studio (VS), choose the default configuration, click File->New->Project and then choose Console Application 

# WRITING FIRST PROGRAM
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

# GETTING USER INPUT 
Console.ReadLine()
static void Main(string[] args){
string yourName;
Console.WriteLine("What is your name?";
yourName = Console.ReadLine();
Console.WriteLine("Welcome " + yourName); // or "Hello {0}", yourName //Note that inputs are strings by default

# TYPE CONVERSION
Convert.ToDouble
Convert.ToInt32
Convert.ToBoolean

static void Main(string[] args){
Console.WriteLine("What is your age?");
int age = Convert.ToInt32(Console.ReadLine());
Console.WriteLine("Your age is {0}", age);


# COMMENTS facilitatesclear understanding
Single line comment //
Multi-line comment /* */

# VAR KEYWORD
var is use to declare variable type automatically
var num = 2; //implicitly typed 
# Constants
store value that cannot change from initial assignment
const double PI = 3.142

Both var and const must be initialized with a value when declared.

# Operators
- substraction (minus)
+ addition (plus)
* multiplication (times)
/ division // returns int value without the remainder, division by 0 is undefined
% modulus (remainder)

# Operator Precedence
determines which gets evaluated first BODMAS (), * / %, + - 
Operators with equal precedence are evaluated from left to right.

# Assignment Operators
int x = 4;
x += 2; // x = x + 2

# Increment ++ and Decrement -- Operator
The increment operator is used to increase an integer's value by one.
int x = 2;
x++; // x = x + 1

# Forms of ++ & -- Opeartor
there are two froms ++x; Prefix and x++; Postfix
Prefix increments the value, and then proceeds with the expression.
Postfix evaluates the expression and then performs the incrementing.

# AREA OF A CIRCLE IN C#
namespace AreaOfCirle
{
    class Program
    {
        static void Main(string[] args)
        {
            const double pi = 3.14;
            double radius;
            radius = Convert.ToDouble(Console.ReadLine());
            var area = pi * (radius * radius);
            Console.WriteLine(area);          
        }
    }
}

# CONDITIONS IN C#
// IF statement
static void Main(string[] args){
int x = 2;
int y = 4;
if (y>x){
Console.WriteLine("y is greater x");
}
}

// Relational Opeartors
<,>,>=,<=,==,!=

// Else clause
if (condition){
 //statements
}
else{
//statements
}
// Example of else
int mark = 85;
if (mark < 59){
Console.WriteLine("failed");
}
else {
Console.WriteLine("Passed");
}

# NESTED IF IN C#
int age = Convert.ToInt32(Console.ReadLine());
if (age > 14)
{
  if(age >= 18){
    Console.WriteLine("You're an adult");
    }
  else{Console.WriteLine("Still a teenager");
    }
}
else{
  if(age > 0){Console.WriteLine("You're a child");}
else{Console.WriteLine("Something is wrong");}
}

// ESLE IF
# SWITCH STATEMENT IN C#
static void Main(string[] args)
        {
            int age = 88;
            switch (age) {
                case 16:
                    Console.WriteLine("Too young");
                    break;
                case 42:
                    Console.WriteLine("Adult");
                    break;
                case 70:
                    Console.WriteLine("Senior");
                    break;
                default:
                    Console.WriteLine("The default case");
                    break;
            }
        }
        
 # While, For and Do WHile Loop
 // WHILE LOOP - executes as long the condition is true
 int x = 1;
 while(int x < 6){
 Console.WriteLine(x);
 x++; // x+=2
 }
 // SHORT FORM
 int num = 0;
 while (++num < 6){
 Console.WriteLine(num);}
 
 // FOR LOOP - executes statement a specific number of times.
 for (int x = 0; x < 10; x++){ //x+=3
  Console.WriteLine(x);
 }
 
 //OR
 for (int x = 10; x > 0; x-=2){
  Console.WriteLine(x);
 }
 
 // 
 int x = 10;
 for(;x>0;x--){}
 //
 int x = 0;
 for (;x<10;){
   //statement;
   x++;
 }
//CREATING AN INFINITE FOR LOOP - for(;;){}

// DO-WHILE LOOP - will run atleast once even when the condition is false // While only execute the staement after testing the condition
int r = 0;
do {
  Console.WriteLine(r);
  r++;
}
while(r<7);

// BREAK
int a = 0;
while (++a < 20){
  if(a == 5){
  break;
  }
  Console.WriteLine(a);
}
// continue - skips
for(int x = 1; x < 10; x++){
  if(x==5)
  continue;
  Console.WriteLine(x);
}

//USING FRO LOOP to print even numbers
for(int x = 1; x <= 10; x++){
 if(x%2 != 0)
 continue;
 Console.WriteLine(x);
}

//LOGICAL OPERATORS
AND = && - all operands must be true
OR = || - any of the operands has to be true
NOT = ! - true when operand is false / works with a single operand

# Condition Operator ?
Console.WriteLine("How old are your?");
int age = Convert.ToInt32(Console.ReadLine());
string msg;
msg = (age >= 18) ? "Welcome" : "Sorry, you are too young to be here";
Console.WriteLine(msg);

# BASIC CALCULATOR
 do {
  Console.Write("x = ");
  string str = Console.ReadLine();
  if (str == "exit")
    break;

  int x = Convert.ToInt32(str);

  Console.Write("y = ");
  int y = Convert.ToInt32(Console.ReadLine());

  int sum = x + y;
  Console.WriteLine("Result: {0}", sum);
}
while (true);

# SUM FROM 1 TO 100
int sum = 0;
for (int x = 1; x<=100; x++){
  sum += x;
}
Console.WriteLine(x);

# Multiple of 3
int number = Convert.ToInt32(Console.ReadLine());
            int n = 1;
            while(n <= number)
            {
                if(n%3==0)
                {
                    Console.WriteLine("*");
                }
                else
                {
                    Console.WriteLine(n);
                }
                n++;
                }
                
 # METHOD IN C#
 A method is a group of statements that perform a particular task
 Main is a built-in method every C# must have
 Console.WriteLine("Enter a number to square");
 int x = Convert.ToInt32(Console.ReadLine());
 int Square(int x){
  int result = x * x;
  return result;
 }
 // void is a basic data type that defines a valueless state i.e. If you do not want your method to return a value
 static void sayHi()
        {
            Console.WriteLine("Hello");
        }
        static void Main(string[] args)
        {
            sayHi();
        }
The static keyword is used to make methods accessible in Main.
 // PARAMETERS
 Method declarations can define a list of parameters to work with.
Parameters are variables that accept the values passed into the method when called.
void Print(int x){
  Console.WriteLine(x);
}
in the above example x is the parameter
argument is the value assigned to the formal parameter x when calling the method in Main
  static void Func(int x)
        {
            Console.WriteLine(x*2);
        }
        static void Main(string[] args)
        {
            Func(5);
  
            Func(12);When calling the method, you can use the parameter names to provide the arguments in any order you like

            Func(42);
        }
// Optional Arguments
static int Pow(int x, int y=2)
{
  int result = 1;
  for (int i = 0; i < y; i++)
  {
    result *= x;
  }
 
  return result;
}
//Named Arguments
Named arguments free you from the need to remember the order of the parameters in a method call. Each argument can be specified by the matching parameter name.
When calling the method, you can use the parameter names to provide the arguments in any order like.

static in Area(int h, int w){
  result = h * w;
  return result;
}
static void Main(string[] args){
  int res = Area(w:5, h:4);
  Console.WriteLine(res);
}
