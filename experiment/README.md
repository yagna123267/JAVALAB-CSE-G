# experiment 1
## TITLE : 1a.) DISPALY PRIMITIVE DATA TYPES
```java
class DefaultPrimitiveType {
    byte primbyte;
    short primshort;
    int primint;
    double primdouble;
    char primchar;
    float primfloat;
    long primlong;
    boolean primboolean;
    public static void main(String args[]) {
        DefaultPrimitiveType dDpt = new DefaultPrimitiveType();
        System.out.println("default value of byte:" + dDpt.primbyte);
        System.out.println("default value of short:" + dDpt.primshort);
        System.out.println("default value of int:" + dDpt.primint);
        System.out.println("default value of double:" + dDpt.primdouble);
        System.out.println("default value of char:" + dDpt.primchar + " '");
        System.out.println("default value of float:" + dDpt.primfloat);
        System.out.println("default value of long:" + dDpt.primlong);
        System.out.println("default value of boolean:" + dDpt.primboolean);
    }
}
```
### Output:
![output for Default Primitvie Data Types](https://github.com/yagna123267/JAVALAB-CSE-G/blob/a47af7b118f71ae4566be34695f6ceb058e8d862/1a%20output.png)

## TITLE : 1b.) Quadratic equation solution
```java
// program code here

import java.util.Scanner;
class QuadraticEquationSolution {
    public static void main(String args[]) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter a value of a:");
        double a = sc.nextDouble();
        System.out.println("Enter a value of b:");
        double b = sc.nextDouble();
        System.out.println("Enter a value of c:");
        double c = sc.nextDouble();
        double D = b * b - 4 * a * c;
        if (D > 0) {
            double x1 = (-b + Math.sqrt(D)) / (2 * a);
            double x2 = (-b - Math.sqrt(D)) / (2 * a);
            System.out.println("Roots are real and distinct:");
            System.out.println("x1 = " + x1);
            System.out.println("x2 = " + x2);
        } 
        else if (D == 0) {
            double y = -b / (2 * a);
            System.out.println("The roots are real and equal:");
            System.out.println("y = " + y);
        } 
        else {
            double real = -b / (2 * a);
            double img = Math.sqrt(-D) / (2 * a);
            System.out.println("Roots are complex:");
            System.out.println("x1 = " + real + " + " + img + "i");
            System.out.println("x2 = " + real + " - " + img + "i");
        }
        sc.close();
    }
}
```
### Output:
![output for quadratic equation](https://github.com/yagna123267/JAVALAB-CSE-G/blob/78fbcf672a431ebdb727727878c938b2a5610b65/1b%20output.png)
## title: 2a) implement class mechanism in java.
```
 class Rectangle {
        double length;
        double breadth;
 double area() {
        return length * breadth;
        }
 double perimeter() {
        return 2*(length + breadth);
        }
 }
class main {
     public static void main(String args[]) {
      Rectangle rect = new Rectangle();
      rect.length = 12;
      rect.breadth = 20;
      double area = rect.area();
      double perimeter = rect.perimeter();
  System.out.println("Area of given Rectangle:"+area);
  System.out.println("perimeter of given rectangle:"+perimeter);
}
}
```
### output:
![output for mechanism in java](https://github.com/yagna123267/JAVALAB-CSE-G/blob/477a1c55d83dab8e1556e52c2df8c42c8dc6656b/2a.output.png)
### title 2b) implement overloading methods in java
```
class sum {
     int sum(int a,int b) {
     return a+b;
     }
     int sum(int a,int b,int c) {
     return a+b+c;
     }
     double sum(double a,double b) {
     return a+b;
     }
   }

 class main {
     public static void main(String args[]) {
      sum S = new sum();
 System.out.println("sum of 2 integers:"+S.sum(30,40));
 System.out.println("sum of 3 integers:"+S.sum(39,56,78));
 System.out.println("summ of real numbers:"+S.sum(20-456,22-564));
 }
}
```
### output:
![output for implement overloading methods in java](https://github.com/yagna123267/JAVALAB-CSE-G/blob/87c6d2b890197a51a0c92079afc9a8827fe5ae1e/2b.output.png)
## title: 2c) implement constructor in java.
```
 class student {
     String Sname;
     int Sage;
     double Smarks;
     student(String name,int age,double marks) {
     Sname = name;
     Sage = age;
     Smarks = marks;
     }
     void display() {
     System.out.println("student name:"+Sname);
     System.out.println("student age:" +Sage);
     System.out.println("student marks:" +Smarks);
     }
}

class main {
     public static void main(String args[]) {
      student S = new student("yagna:",19,600);
      S.display();
}
}
```
### output:
![output for implement constructor in java](https://github.com/yagna123267/JAVALAB-CSE-G/blob/f15f8a1075dfaf6358cd64611af8a8fb9e1fc50e/2c.output.png)
## title: additional experiment 2 :fibanocis series.
```
class Fibonacis {
     int firstNumber;
     int secondNumber;
     int thirdNumber;
     int sum;
     int sizeofFibsequence;
     Fibonacis(int size) {
     firstNumber = 0;
     secondNumber = 1;
     thirdNumber = 0;
     sum = 0;
     sizeofFibsequence = size;
   }
     void generateFibsequence() {
       while(sizeofFibsequence > 0) {
         if(sizeofFibsequence == 1)
       System.out.print(firstNumber + ".");
class Fibonacis {
     int thirdNumber;
     int sum;
     int sizeofFibsequence;
     Fibonacis(int size) {
     firstNumber = 0;
     secondNumber = 1;
     thirdNumber = 0;
     sum = 0;
     sizeofFibsequence = size;
   }
     void generateFibsequence() {
       while(sizeofFibsequence > 0) {
         else
      System.out.print(firstNumber + ",");
      sizeofFibsequence--;
      sum += firstNumber;
      thirdNumber = firstNumber + secondNumber;
      firstNumber = secondNumber;
      secondNumber = thirdNumber;
      }
    }
    int getFibsum() {
        return sum;
      }
    }
import java.util.Scanner;
  class main {
     public static void main(String args[]) {
       System.out.print("enter the sizeof the sequence:");
       Scanner Sc = new Scanner(System.in);
       int size = Sc.nextInt();
       if(size > 0) {
          Fibonacis Fib = new Fibonacis(size);
      System.out.print("Fibonacciseries are:");
                 Fib.generateFibsequence();

      System.out.println("the sum of Fibonacciseries are:" + Fib.getFibsum());
}
      else
        System.out.println("Fibonacci sequence and sum cannot be calculated:");
      }
    }
```
## output:
![output for fibanocis series](<img width="489" height="94" alt="image" src="https://github.com/user-attachments/assets/b97b8556-cad7-49d6-95e3-242b3bb56bf1" />)























