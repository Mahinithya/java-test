# java-test
Java Test Questions
Part 1
Two marks questions (Totally 10 question: 10 X 2 = 20)
1.	What are instance and local variables? Give some examples.
    If we declare any variable inside the class but outside the method is known as instance variable.
Example: class Exam
{ 
Int x=20
Void main()
{ 
Int a=40
}
Here x is instance variable.

Local variables:
If we declare any variables inside the method is known as local variable.
In above program “a” is local variable.

2.	Can a main() method be overloaded?
Yes ,we can overload the main method in compile time polymorphism.

3.	What is the purpose of declaring a variable as final?
Once we declare the variable as final we cannot change the value of that variable.

4.	What is an Abstract Class and what is it’s purpose? Provide some example
If   any class having at least one abstract method, that class   should be abstract class.  Abstract   method is nothing but only declaration, it doesn’t contain any definition.
E.g: Void read();

A abstract class also contains the non abstract   method. We can use the key word “abstract “ to create the abstract  class.
E.g:
Abstract class Vehicle
{
Abstract void colour ();
Void  fast()
{
System.Out.println(“fast”);
}
}
Class Car extends Vechile
{
Void colour()
{
System.out.println(“red”);
}
}
public static void main(String args[])
{
Car c=new Car ();
c.fast();
c.colour();
}
}

5.	Why is an Interface be able to extend more than one Interface but a Class can't extend more than one Class?
In   multiple inheritance  concept if the same method is in two parent class means the main method can’t be identify in which class method it indicates actually. Hence we are moving to interface.
In interface concept even we can extend the N number of interfaces finally we create a class and declare & define the method as “public”. Hence the interface can be extend.

6.	What is an abstract method? Provide some example
Abstract method is nothing but only provide the declaration and not definition.
We are using the Keyword “abstract “ to declare the abstract method.

E.g:  abstract void read();

7.	What do you understand by private, protected and public?
We are going to provide some access to a variable or method or class is known as Access modifier.
It has 3 types.
Public: we can use anywhere in the program.

Private: we can use within the class.

Protected: we can use within the package.

8.	What is the difference between method overriding and method overloading?
Same method name with different number of arguments is known as method overloading.
Same method name with same number of arguments in both parent and child class is known as method overriding.

9.	How are this() and super() keywords used ?

This keyword is used to refer current class object.
Super keyword is used to immediately refer the parent class object.

10.	What is difference between checked and unchecked exception?
Which are all exceptions checked in compile time is called as checked exception.
Which are all exceptions checked in run time is called as unchecked exception.

Part 2: Predict the output of following Java Programs.
Three marks questions (Totally 5 question: 5 X 3 = 15)
class Test {
    int x, y;
}
class Main {
    public static void main(String args[]) {
        Test t = new Test();
        System.out.println(t.x + " " + t.y);
    }
}

o/p Error will occur.

=========================================================
class Calculation{  
void sum(int a,int b){System.out.println(a+b);}  
 void sum(int a,int b,int c){System.out.println(a+b+c);}  
  public static void main(String args[]){  
Calculation obj=new Calculation();  
obj.sum(10,10,10);  
obj.sum(20,20);   }  }  

output: 30
              40

======================================================
class Bike{  
final int speedlimit=90;
void run(){  
 speedlimit=400;  
 }  
 public static void main(String args[]){  
 Bike obj=new  Bike();  
 obj.run();  
 }  
}

Output: error will occur.

======================================================
class A{  
void msg(){System.out.println("Hello");}  
}  
class B{  
void msg(){System.out.println("Welcome");}  
}  
class C extends A,B
   
Public Static void main(String args[]){  
   C obj=new C();  
   obj.msg
}  
}  
Output: Error ll occur.
=======================================================
abstract class Bank{    
abstract void getRateOfInterest();    
}    
class SBI extends Bank{    
void getRateOfInterest(){
System.out.println(“8”);
}    
}    
class PNB extends Bank{    
void getRateOfInterest(){
System.out.println(“7”);
}    
}    
class TestBank{    
public static void main(String args[]){    
Bank b=new SBI();    
b.getRateOfInterest();        
}
}
o\p: error will occur.

Part 3: Write the program for following scenarios

Five marks questions (Totally 3 question: 3 X 5 = 15)
1.	Write the program for student marks calculation using object and class.

2.	Write the program for your choice using both class and interface (using inheritance concept)

Abstract class Vechicle
{
abstract void speed();
Void fast
{
System.Out.println(“fast”);
}
}
class Bike extends Vechicle
{
Void speed()
{
System.out.println(“speed”);
}
}
public static void main(String args[])
{
Bike b=new bike();
b.speed();
b.fast();
}
}

3.	Write the program for your choice using polymorphism concept
                     	Method overloading(By changing the no of arguments)
class A
{void sub(int a,int b)
{
System.Out.println(a-b);
}
Void sub(int a,int b,int c)
{
System.Out.println(a-b-c)
}
public static void main(String args[])
{
A.obj=new A();
Obj.sub(100,50);
Obj.sub(100,50,25)
}
}	
              	Method overloading(By changing the data type in argument)
class B
{
Void add(int a,int b)
{
System.out.println(a-b);
}
Void add(string location)
{
System.Out.println(location);
}
public static void main(String args[])
{
B t=new B();
t.add(10,20);
t.add(Thiruvanmaiyur);
}
}










