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

//PASSING ARGUMENTS
There are three ways to pass arguments to a method when the method is called: By value, By reference, and as Output.
// BY VALUE
static void Sqr(int x){
  x=x*x;
}
static void Main(string[] args){
  int a = 3;
  Sqr(a);
  Console.WriteLine(a); // Outputs 3
}

// REFERENCE
static void Sqr(ref int y){
  y = y*y;
}

static void Main(string[] args){
  int d = 2;
  Sqr(ref d);
  Console.WriteLine(d); // 4
}
// SWAP
void Swap(ref int x, ref int y){
  int temp;
  temp = x;
  x = y;
  y = temp;
}
// Passing by OUPUT

Output parameters are similar to reference parameters, except that they transfer data out of the method rather than accept data in. They are defined using the out keyword.
static void GetValues(out int a, out int b){
  a = 34;
  b = 45;
}
static void Main(string[] args){
  int x, y;
  GetValues(out x, out y);
// gives x and y the value of 34, 45
}

// METHOD OVERLOADING
Method overloading is when multiple methods have the same name, but different parameters.
void Print(int a){
  Console.WriteLine("Value: "+a);
}
void Print(double a){
  Console.WriteLine("Value: "+a);
}
// a now works for both int and double - same method different parameters

void Print(string label, double a){
  Console.WriteLine(label +a);
}
//RECURSION
A recursive method is a method that calls itself. - Factotial
static void Fact(int a){
 if (a == 1){
 return 1; // exit condition
 }
 retrun a * Fact(a-1);
}
# Making a Puramid in C#
an algorithm is the step by step logic required for the solution to a problem
using System;
namespace MakingPyramid
{
  class Program
  {
    static void DrawPyramid(int n)
    {
      for (int i=1; i<=n; i++)
      {
        for (int j=i; j<=n; j++)
        {
          Console.Write("  "); // displays the space on each row
        }
        for (int k=1; k<=2*i-1; k++)
        {
          Console.Write("*"+" "); // displays the required number of stars on each row
        }
        Console.WriteLine(); // moves the cursor to the next row
      }
    }
    static void Main(string[] args)
    {
      DrawPyramid(5);
    }
  }
}

Level Points


Passing the first level of a video game awards the player 1 point. For each subsequent level passed, the points awarded increment by 1 (2 for the 2nd level, 3 for the 3rd, and so on).
The program you are given takes the number of passed levels as input. Complete the given function to take that number as an argument, and recursively calculate and return the total number of points given for all passed levels.
namespace LevelPoints
{
    class Program
    {
        static void Main(string[] args)
        {
            int levels = Convert.ToInt32(Console.ReadLine());

            Console.WriteLine(Points(levels));
        }

        
        static int Points(int levels)
        {
            //your code goes here
            if (levels == 1){
                return 1;}
            return levels + Points(levels - 1);
            
             
        }

    }

}

# CLASSES AND OBJECTS IN C#
class is a data type that defines a set of variables and methods for a declared object. class contains properties and methods. Objects are instance of a class.
// To use custom data types, you need to define a class. class is the blueprint of creating different objects. The process of creating objects is called instantiation
The characteristics of an object are called properties. This describes the current state of an object.

// C# has two ways of storing data: by reference and by value.
The built-in data types, such as int and double, are used to declare variables that are value types. Their value is stored in memory in a location called the stack.

// Reference types are used for storing objects. For example, when you create an object of a class, it is stored as a reference type.
Reference types are stored in a part of the memory called the heap.
When you instantiate an object, the data for that object is stored on the heap, while its heap memory address is stored on the stack.
That is why it is called a reference type - it contains a reference (the memory address) to the actual object on the heap.

Stack is used for static memory allocation, which includes all your value types, like x.
Heap is used for dynamic memory allocation, which includes custom objects, that might need additional memory during the runtime of your program.

class Person
{
  int age;
  string name;
  public void SayHi()
  {
    Console.WriteLine("Hi");
  }
}
static void Main(string[] args){
  Person p1 = new Person();
  p1.SayHi();
  p1.age = 45;
  p1.name = "Ridwan";
  Console.WriteLine(p1.age);
  }
 Access modifiers are keywords used to specify the accessibility of a member. public can be accessed from outside the class, as long as it's anywhere within the scope of the class object. You can also designate class members as private or protected
 
Encapsulation is also called information hiding. encapsulation is the idea of keeping together and protecting entity.  It simply combining members together within a class and restricting access to the inner workings of that class. Encapsulation is implemented by using access modifiers. An access modifier defines the scope and visibility of a class member. It allows you to hide detaails of a class realization.

C# supports the following access modifiers: public, private, protected, internal, protected internal. the public access modifier makes the member accessible from the outside of the class.
The private access modifier makes members accessible only from within the class and hides them from the outside.
In summary, the benefits of encapsulation are:
- Control the way data is accessed or modified.
- Code is more flexible and easy to change with new requirements.
- Change one part of code without affecting other parts of code.
class BankAccount {
        private double balance=0;
        public void Deposit(double n) {
            balance += n;
        }
        public void Withdraw(double n) {
            balance -= n;
        }
        public double GetBalance() {
            return balance;
        }
    }
    class Program
    {
        static void Main(string[] args)
        {
            BankAccount b = new BankAccount();
            b.Deposit(199);
            b.Withdraw(42);
            Console.WriteLine(b.GetBalance());
        }
    }
// CONSTRUCTORS
A class constructor is a special member method of a class that is executed whenever a new object of that class is created.
A constructor has exactly the same name as its class, is public, and does not have any return type.
class Person
{
  private int age;
  public Person()
  {
    Console.WriteLine("Hi there");
  }
}
static void Main(string[] args){
  Person p = new Person();
}
 This can be useful in a number of situations. For example, when creating an object of type BankAccount, you could send an email notification to the owner.
The same functionality could be achieved using a separate public method. The advantage of the constructor is that it is called automatically.
Constructors can be very useful for setting initial values for certain member variables.
A default constructor has no parameters. However, when needed, parameters can be added to a constructor. This makes it possible to assign an initial value to an object when it's created
Constructors can be overloaded like any method by using different numbers of parameters.
 class Program
    {
        class Person
        {
            private int age;
            private string name;
            public Person(string nm)
            {
                name = nm;
            }
            public string getName()
            {
                return name;
            }
        }
        static void Main(string[] args)
        {
            Person p = new Person("David");
            Console.WriteLine(p.getName());
        }
    }
A property is a member that provides a flexible mechanism to read, write, or compute the value of a private field. Properties can be used as if they are public data members, but they actually include special methods called accessors.
The accessor of a property contains the executable statements that help in getting (reading or computing) or setting (writing) a corresponding field. Accessor declarations can include a get accessor, a set accessor, or both.
class Person
{
  private string name; //field

  public string Name //property
  {
    get { return name; }
    set { name = value; }
  }
}
The Person class has a Name property that has both the set and the get accessors.
The set accessor is used to assign a value to the name variable; get is used to return its value.
value is a special keyword, which represents the value we assign to a property using the set accessor.
The name of the property can be anything you want, but coding conventions dictate properties have the same name as the private field with a capital letter.
Once the property is defined, we can use it to assign and read the private member:
The property is accessed by its name, just like any other public member of the class.
class Program
    {
        class Person
        {
            private string name;
            public string Name
            {
                get { return name; }
                set { name = value; }
            }
        }
        static void Main(string[] args)
        {
            Person p = new Person();
            p.Name = "Bob";
            Console.WriteLine(p.Name);
        }
    }
Any accessor of a property can be omitted.
For example, the following code creates a property that is read-only:
// skipping the set accessor creates a read-only property
class Person
{
  private string name;
  public string Name
  {
    get { return name; }
  }
}
A property can also be private, so it can be called only from within the class.
So, why use properties? Why not just declare the member variable public and access it directly?
With properties you have the option to control the logic of accessing the variable.
For example, you can check if the value of age is greater than 0, before assigning it to the variable:
class Person
{
  private int age=0;
  public int Age
  {
    get { return age; }
    set {
      if (value > 0)
        age = value;
    }
  }
}
You can have any custom logic with get and set accessors.
// Auto-Implemented Properties
When you do not need any custom logic, C# provides a fast and effective mechanism for declaring private members through their properties.
For example, to create a private member that can only be accessed through the Name property's get and set accessors, use the following syntax:
public string Name { get; set; }
As you can see, you do not need to declare the private field name separately - it is created by the property automatically. Name is called an auto-implemented property. Also called auto-properties, they allow for easy and short declaration of private members.
We can rewrite the code from our previous example using an auto-property:
 class Program
    {
        class Person
        {
            public string Name { get; set; }
        }
        static void Main(string[] args)
        {
            Person p = new Person();
            p.Name = "Bob";
            Console.WriteLine(p.Name);
        }
    }






