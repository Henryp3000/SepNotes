# SepNotes

Notes App DEV

Chapter 1




The Anatomy of a class 

Public static void main (String[]  args) {
// your code goes here 

// public open for everyone to see
// the class
// the name of this class “MyFirstApp”
// opening curly brace 

Public class MyFirstApp{


// public open for everyone to see
//
// void is the return type
// main is the method
//(String is the argument)

Public static void main (String[]  args) {	
System.out.print( ”I Rule”

}	

What can you do in the main method?
You can make the computer do something
•	Statements
•	Loops
•	Branching

                    
                      
                             



Statements: declarations, assignments, method calls, etc. 
          int x = 3;
          String name = “Dirk”;
          x = x * 17;
          System.out.print(“x is ” + x);
          double d = Math.random();
          // this is a comment


       Loops: for and while 
                while (x > 12) {
x = x - 1; } 
                for (int x = 0; x < 10; x = x + 1) {
                   System.out.print(“x is now ” + x);
                }
                 
Branching: if/else tests if (x == 10) { 
          System.out.print(“x must be 10”);
       } else {
       }  System.out.print(“x isn’t 10”);
       if ((x < 3) & (name.equals(“Dirk”))) {
       }  System.out.println(“Gently”);
       System.out.print(“this line runs no matter what”);







Chapter 2


Supper Class 
// from the supper claas you can have sub classes
// extend allows sub classes to have access to the superclass

Ex. Would be Shape
Supper class is like the parent 


Sub classes
Are the children of the super class
Ex. 
•	Circle 
•	Triangle
•	Square



Pg:34

When designing a class, think about the object you want to create from that class type.

The difference between a class and an object.
A class is not an object but is used to construct them

•	Things an object knows about itself are called instance variables. 
•	Think of instance as another way of saying object. 
•	Things an object can do are called methods. 
Example: Alarm
•	Alarm mode 
•	Alarm time
Song
Varables: what it know 
•	Title
•	 Artist
Methods: what it does
•	Set Title
•	set Artist
•	play




A class is a blueprint for an object.” Tell the computer how to make a object of the particular type”











Chapter 3

Variables come in two flavors: primitive and reference
•	a primitive variable's information is stored as the value of that variable,
•	a reference variable holds a reference to information related to that variable.

variables must have a type 
variables must have a name 

Example of a Primitive Variable 	
Int = 3



Declare a reference variable 
Example of a reference variable
Dog myDog = new Dog(); 
The Dog object itself does not go into
the variable! 
Tells the program to make  space for a
reference variable “my dog”
 The reference variable
is, forever, of type Dog. In other words,



Create an object 
Dog myDog = new Dog(); 

Link the object and the reference 
Dog myDog = new Dog(); 
Assigns the new Dog to the reference variable myDog. In other words, 

Make an array of Dogs 
lass Dog {
String name;
public static void main (String[] args) { 
// make a Dog object and access it 
Dog dog1 = new Dog(); dog1.bark(); dog1.name = “Bart”; 
// now make a Dog array 
Dog[] myDogs = new Dog[3]; 
// and put some dogs in it 
myDogs[0] = new Dog(); myDogs[1] = new Dog(); myDogs[2] = dog1; 
// now access the Dogs using the array // references
myDogs[0].name = “Fred”; myDogs[1].name = “Marge”; 
// Hmmmm... what is myDogs[2] name? 
System.out.print(“last dog’s name is “); System.out.println(myDogs[2].name); 
// now loop through the array // and tell all dogs to bark int x = 0;
while(x < myDogs.length) { 
myDogs[x].bark(); 
x = x + 1; } 
} 
public void bark() { System.out.println(name + “ says Ruff!”); 
} 
public void eat() { } 
public void chaseCat() { } 












Chapter 4
a class describes what an object knows and what an object does 
A class is the blueprint for an object. 
A method uses parameters. 
A caller passes arguments. 


Encapsulation
The purpose: is to make sure that "sensitive" data is hidden from users.

Getters and Setters
private variables can only be accessed within the same class (an outside class has no access to it). However, it is possible to access them if we provide public get and set methods.
The get method returns the variable value, 
The set method sets the value.







