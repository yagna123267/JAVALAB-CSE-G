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
![output for fibanocis series](https://github.com/yagna123267/JAVALAB-CSE-G/blob/d88fe64cbf0a0acde88fe79b424c83a81dccaf53/experiment/Screenshot%202026-01-06%20095921.jpgt.jpg)
## title: experiment 3a) :Student and main.
```  class Student {
        String name;
        int age;
        double marks;
        Student() {
        }
        Student(String name,int age,double marks) {
                this.name = name;
                this.age = age;
                this.marks = marks;
                }
                void display() {
                System.out.println("name:" +name);
                System.out.println("age:" +age);
                System.out.println("marks:" +marks);
                }
             }
   class main {
     public static void main(String args[]) {
            Student std = new student();
             Std.display();
            student std1 = new student("yagna", 12,400);
             Std1.display();
       }
      }
```
## output :
![output for student ](https://github.com/yagna123267/JAVALAB-CSE-G/blob/c4595132e7b378e4ed2888971c7ea1446df8b85f/3a.output.png)
## title : 3b) Binarysearch
```
import java.util.Scanner;

class Binarysearch {
    int list[];
    int size;

    Binarysearch(int size) {
        this.size = size;
        list = new int[size];
    }

    void setlist() {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the list items in Ascending order:");
        
        for (int i = 0; i < size; i++) {
            System.out.println("Enter value " + (i + 1) + ": ");
            list[i] = sc.nextInt();
        }
    }

    void getlist() {
        for (int i = 0; i < size; i++)
            System.out.print(list[i] + ",");
        System.out.println("\b\b.");
    }

    int Binarysearch(int key) {
        int low = 0;
        int high = list.length - 1;

        while (low <= high) {
            int mid = (low + high) / 2;

            if (list[mid] == key)
                return mid;

            else if (list[mid] < key)
                low = mid + 1;

            else
                high = mid - 1;
        }

        return -1; 
    }
}
import java.util.Scanner;

class main {
    public static void main(String args[]) {
        Scanner sc = new Scanner(System.in);

        Binarysearch bs = new Binarysearch(10);

        bs.setlist();
        bs.getlist();

        System.out.println("Enter the key to search: ");
        int key = sc.nextInt();

        int index = bs.Binarysearch(key);

        if (index == -1)
            System.out.println("Key item does NOT exist.");
        else
            System.out.println("Key item exists at index: " + index);
    }
}
```
## output:
![output for binarysearch](https://github.com/yagna123267/JAVALAB-CSE-G/blob/0989a1838437434cad9a48c834f3f2faeaf873ce/3b.output.png)
## title 3c:bubblesort
```
  class Bubblesort {

    void bubbleSort(int arr[]) {
        int n = arr.length;
        for(int i = 0; i < n - 1; i++) {
            for(int j = 0; j < n - i - 1; j++) {
                if(arr[j] > arr[j + 1]) {
                    int temp = arr[j + 1];
                    arr[j + 1] = arr[j];
                    arr[j] = temp;
                }
            }
        }
    }
}
import java.util.Scanner;
class main {
   public static void main(String args[]) {
      System.out.print("enter the size of array:");
      Scanner sc = new Scanner(System.in);
      int size = sc.nextInt();
      int integer[] = new int[size];
      for(int i= 0; i < size; i++) {
           System.out.println("enter the value of integer at index" + (i+1) + ":");
           integer[i] = sc.nextInt();
        }
        Bubblesort bs = new Bubblesort();
        bs.Bubblesort(integer);
        System.out.print("the sorted integers:");
        for(int i=0;i<size;i++) 
        System.out.print(integer[i] + ",");
        System.out.println("\b\b.");
     }
  }
```
## output:
![output for bubblesort](https://github.com/yagna123267/JAVALAB-CSE-G/blob/15db45c5bb60ddab7bcab103a004ef9e1a49a330/3c.output.png)
## title : 4a) single inheritance
```
 class Person {
      String name;
      int age;
      Person(String name, int age) {
           this.name = name;
           this.age = age;
     }
     void displayPersonDetails() {
      System.out.println("Name:" +name);
      System.out.println("Age:" +age);
   }
 }


class Employee extends Person {
        double annualSalary;
        int yearofJoining;
        String nationalInsuranceNumber;
        Employee(String name,int age,double annualSalary,int yearofJoining,String nationalInsuranceNumber) {
                super(name,age);
                this.annualSalary = annualSalary;
                this.yearofJoining = yearofJoining;
                this.nationalInsuranceNumber =nationalInsuranceNumber;
       }
       void displayEmployeeDetails() {
            displayPersonDetails();
       System.out.println("AnnualSalary:" +annualSalary);
       System.out.println("YearofJoining:" +yearofJoining);
       System.out.println("NationalInsuranceNumber:" +nationalInsuranceNumber);
     }
  }



class TestEmployee {
     public static void main(String args[]) {
  Employee emp1 = new Employee("yagna",20,100000,2029,"NI807468YT");
             emp1.displayEmployeeDetails();
           }
}


```
## output:
![output for single inheritance](https://github.com/yagna123267/JAVALAB-CSE-G/blob/cb5d79b00a67c7e4c671591b8c3e8f90ed03eed5/experiment/4a.output.png)
## title: 4b) multilevel inheritance 
```
 class Bicycle {
     String PedalType;
     void showBicycleInfo() {
   System.out.println("This is a bicycle with Pedals.");
   System.out.println("PedalType:" + PedalType);
  }
}
 class Motorbike extends Bicycle {
       int engineCapacity;
   void showMotorbikeInfo() {
   System.out.println("This Motorbike has an engine.");
   System.out.println("engineCapacity:" +engineCapacity + "cc");
  }
}
  class Electricbike extends Motorbike {
      int batteryCapacity;
    void showElectricbikeInfo() {
   System.out.println("This electric bike has an electric motor and battery.");
   System.out.println("batteryCapacity:" + batteryCapacity + "Wh");
   }
}
class TestVehicle {
     public static void main(String args[]) {
     Electricbike ebike = new Electricbike();
     ebike.PedalType = "standard Pedals:";
     ebike.engineCapacity = 268;
     ebike.batteryCapacity = 666;
     ebike.showBicycleInfo();
     ebike.showMotorbikeInfo();
     ebike.showElectricbikeInfo();
   }
}
```
## output:
![output for multilevel inheritance](https://github.com/yagna123267/JAVALAB-CSE-G/blob/72b7a2d8feeaecac5e74449dc7b2777079de56a1/experiment/4b.output.png)
## title 4c) dimensions
```
    abstract class Figure {
      double dim1;
      double dim2;
      Figure(double dim1,double dim2) {
      this.dim1 = dim1;
      this.dim2 = dim2;
      }
 abstract double area();
 }
  abstract class Figure {
      double dim1;
      double dim2;
      Figure(double dim1,double dim2) {
      this.dim1 = dim1;
      this.dim2 = dim2;
      }
 abstract double area();
 }
  class Triangle extends Figure {
      Triangle(double base,double height) {
              super(base,height);
      }
     double area() {
            double result = 0.5*dim1*dim2;
            return result;
     }
}
  class TestFigure {
       public static void main(String args[]) {

       Figure f1 = new Rectangle(99.9,66.6);
       Figure f2 = new Triangle(88.8,55.5);


       System.out.println("Area of Rectangle = " +f1.area());
       System.out.println("Area of Triangle = " +f2.area());
       }
}
```
## output:
![output for Figure](https://github.com/yagna123267/JAVALAB-CSE-G/blob/e5a95dfb1e072e25edcd3ba9235b85333cc47a8e/experiment/4c.outputt.png)
## title Insert substring
```
import java.util.Scanner;
   class InsertSubstring {
      public static void main(String args[]) {
        Scanner SC = new Scanner(System.in);
     System.out.print("MainString:");
     String mainString = SC.nextLine();
     System.out.print("SubString:");
     String Substring = SC.nextLine();
     System.out.print("Position:");
     int Position = SC.nextInt();
     if(Position < 0 ||Position > mainString.length()) {
      System.out.print("Invalid Position:");
     } else {
      String FirstPart = mainString.substring(0,Position);
      String SecondPart = mainString.substring(Position);
      String resultString = FirstPart + Substring + SecondPart;
       System.out.println("The resultant string: " + resultString);
   }
 SC.close();
  }
}
```
output:
![output for insert substring](https://github.com/yagna123267/JAVALAB-CSE-G/blob/491639fd6009618e977fcef8520affd83f12ca3d/substring.png)


## title Palindrome
```
 import java.util.Scanner;
   class PalindromeCheck {
    public static void main(String args[]) {
      Scanner SC = new Scanner(System.in);
    System.out.print("Enter a String:");
    String str = SC.nextLine();
    int start = 0;
    int end = str.length()-1;
    while(start < end) {
        if(str.charAt(start) != str.charAt(end)) {
    System.out.println("The String \"" + str + "\" is not a Palindrome");
     SC.close();
     return ;
   }
   start ++;
   end --;
 }
 System.out.println("The String \"" + str + "\" is a Palindrome");
 SC.close();
   }
 }
```
output:
![output for palindrome](https://github.com/yagna123267/JAVALAB-CSE-G/blob/c6eaeaec56e17eb47948e1d6e8c09c4ca33148d2/tt.jpg)

## title perfect number
```
 import java.util.Scanner;
   class PerfectNumber {
     public static void main(String args[]) {
       Scanner SC = new Scanner(System.in);
      System.out.print("Enter a number:");
      int num = SC.nextInt();
      int sum = 0;
      for(int i=1;i<num-1;i++) {
         if(num %i == 0) {
             sum =sum +i;
          }
      }
     if(sum == num) {
       System.out.println(num + "is a PerfectNumber.");
     } else {
       System.out.println(num + "is not a PerfectNumber.");
       }
     }
}

```
output:
![output for perfect number](https://github.com/yagna123267/JAVALAB-CSE-G/blob/d1053de1bddb9a0620b3697310a0f053de5254ab/Screenshot%202026-01-31%20162330.jpg)
## title : 5a) sortable
```
interface Sortable {
    void sort(int arr[]);
}
class BubbleSort implements Sortable {
    public void sort(int arr[]) {
        int n = arr.length;
        for (int i = 0; i < n - 1; i++) {
            for (int j = 0; j < n - i - 1; j++) {
                if (arr[j] > arr[j + 1]) {
                    int temp = arr[j];
                    arr[j] = arr[j + 1];
                    arr[j + 1] = temp;
                }
            }
        }
    }
}
class SelectionSort implements Sortable {
    public void sort(int arr[]) {
        int n = arr.length;
        for (int i = 0; i < n - 1; i++) {
            int min = i;
            for (int j = i + 1; j < n; j++) {
                if (arr[j] < arr[min]) {
                    min = j;
                }
            }
            int temp = arr[min];
            arr[min] = arr[i];
            arr[i] = temp;
        }
    }
}
```
![output for Sortable](https://github.com/yagna123267/JAVALAB-CSE-G/blob/5926dcd6b53faf7e78d663bd5702ff8e0c17b4af/exp5a.png)

 ## title: 5b) Vehicle plymorphism:
 ```
  class Vehicle {
      void run() {
         System.out.println("Vehicle is running");
        }
     }
class Car extends Vehicle {
          void run() {
       System.out.println("Car is running on four wheels");
      }
   }
class Bike extends Vehicle {
        void run() {
    System.out.println("Bike is running on two wheels");
   }
}
public class TestVehicle {
    public static void main(String[] args) {
        Vehicle v;
        v = new Car();
        v.run();
        v = new Bike();
        v.run();
        v = new Vehicle();
        v.run();
    }
}
```
![output for](https://github.com/yagna123267/JAVALAB-CSE-G/blob/164f1e2a4c15d79fd328e727a80e1f1b32f0cf86/exp5b.png)

## title: 5c) StringBufferDelete 
```
 class StringBufferDelete {
    public static void main(String[] args) {
        StringBuffer sb = new StringBuffer("Java Programming");
        System.out.println("Original String: " + sb);
        sb.deleteCharAt(4);
        System.out.println("After deleting character at index 4: " + sb);
        sb.delete(0, 4);
        System.out.println("After deleting characters from index 0 to 4: " + sb);
    }
}
```
![output for](https://github.com/yagna123267/JAVALAB-CSE-G/blob/95dbf7b035aa607d166415a9e90fd93ce657c3b9/exp5c.png)
## 6a)
```
import java.util.Scanner;

class ExceptionHandling {
    public static void main(String args[]) {

        Scanner sc = new Scanner(System.in);

        System.out.println("Enter the size of array:");
        int n = sc.nextInt();

        int[] arr = new int[n];

        for (int i = 0; i < n; i++) {
            System.out.println("Enter an element at index " + i + ":");
            arr[i] = sc.nextInt();
        }

        System.out.println("Enter an index to access:");
        int index = sc.nextInt();

        try {
            System.out.println("Enter an element at index " + index + " is: " + arr[index]);
        } catch (ArrayIndexOutOfBoundsException e) {
            System.out.println("Invalid index! Please enter index between 0 and " + (n - 1));
        }

        sc.close();
    }
}

```
## output:
![output for 6a](https://github.com/yagna123267/JAVALAB-CSE-G/blob/caedb566b2872f9cb82900966db15d5d66042404/6a.png)


## 6b)
```
import java.util.Scanner;
import java.util.InputMismatchException;
  class MultipleCatch {
   public static void main(String args[]) {
    Scanner sc = new Scanner(System.in);
    int [] arr = {1,2,3,4,5};
      try {
       System.out.println("Enter first number:");
          int a = sc.nextInt();
       System.out.println("Enter second number:");
          int b = sc.nextInt();
          int result = a/b;
      System.out.println("Result =" +result);
      System.out.println("Enter index to access array element:");
          int index = sc.nextInt();
      System.out.println("Element at index = " +arr[index]);
         }
       catch(ArithmeticException e) {
        System.out.println("Error: Division by zero is not allowed.");
        }
        catch(InputMismatchException e) {
          System.out.println("Error: Please enter numeric values only.");
          }
          catch(ArrayIndexOutOfBoundsException e) {
            System.out.println("Some other error occured.");
            }
            System.out.println("Program continues...");
          }
        }
```
## output:
![output for 6b](https://github.com/yagna123267/JAVALAB-CSE-G/blob/0b8078d22a3a80b367a57fdf9cbf6efb2e7bc215/6b.png)
## 6c)
```
import java.util.Scanner;

class BuiltinException {
    public static void main(String args[]) {

        Scanner sc = new Scanner(System.in);

        try {
            System.out.print("Enter an integer to divide 100: ");
            int n = sc.nextInt();
            int result = 100 / n;
            System.out.println("Result = " + result);

            int arr[] = new int[3];
            System.out.println("The array element of index 5 is " + arr[5]);

            System.out.print("Enter a number as text: ");
            String s = sc.next();
            int a = Integer.parseInt(s);
        }

        catch (ArithmeticException e) {
            System.out.println("Arithmetic Exception: Division by zero " + e);
        }

        catch (ArrayIndexOutOfBoundsException e) {
            System.out.println("Array Index Out Of Bounds Exception: Invalid index");
        }

        catch (NumberFormatException e) {
            System.out.println("Number Format Exception: Invalid numeric format");
        }

        catch (Exception e) {
            System.out.println("Some other exception occurred: " + e);
        }

        sc.close();
    }
}
```
## output:
![output for 6c](https://github.com/yagna123267/JAVALAB-CSE-G/blob/92cccf6cf0e56f603faaaa33c80c3f1122509a1b/6c.png)
## 7a
```
class InvalidCountryException extends Exception {
          InvalidCountryException() {
              super();
              }
              InvalidCountryException(String message) {
              super(message);
              }
            }
class UserRegion {

    void registerUser(String userName, String userCountry) throws InvalidCountryException {

        if (!userCountry.equals("India")) {
            throw new InvalidCountryException("User outside India cannot be registered");
        } else {
            System.out.println("User registration done successfully");
        }
    }

    public static void main(String args[]) {

        UserRegion ur = new UserRegion();

        try {
            ur.registerUser("Ravi", "USA");
        }
        catch (InvalidCountryException e) {
            System.out.println(e.getMessage());
        }
    }
}
```
## OUTPUT:
![output for 7a ](https://github.com/yagna123267/JAVALAB-CSE-G/blob/a342a636412c04c52bf84e40841d15315bc2d645/7a%20java.png)
## 7b
```
class GoodMorningThread extends Thread {
    public void run() {
        while (true) {
            System.out.println("Good Morning");
            try {
                Thread.sleep(1000); 
            } catch (InterruptedException e) {
                System.out.println(e);
            }
        }
    }
}
  class HelloThread extends Thread {
     public void run() {
          while(true) {
            System.out.println("Hello");
         try {
            Thread.sleep(2000);
         }
         catch(InterruptedException e) {
               System.out.print(e);
           }
        }
    }
  }
   class WelcomeThread extends Thread {
         public void run() {
          while(true) {
        System.out.println("Welcome");
         try {
           Thread.sleep(3000);
         }
         catch(InterruptedException e) {
         System.out.print(e);
         }
       }
     }
   }
  class TestThreads {
     public static void main(String args[]) {
            GoodMorningThread t1 = new GoodMorningThread();
            HelloThread t2 = new HelloThread();
            WelcomeThread t3 = new WelcomeThread();


            t1.start();
            t2.start();
            t3.start();
           }
         }
```
![output for 7b ](https://github.com/yagna123267/JAVALAB-CSE-G/blob/a342a636412c04c52bf84e40841d15315bc2d645/7b%20java.png)
## 7c
```
  class LongRunningTask extends Thread {
        public void run() {
      System.out.println("Long running task started...");
      try {
            for(int i=1;i<= 5;i++) {
      System.out.println("Working..." +i);
            Thread.sleep(1000);
        }
     }
      catch(InterruptedException e) {
       System.out.println(e);
   }
  System.out.println("Long running task completed!");
      }
     }
public class ThreadDemo {
    public static void main(String[] args) {

        LongRunningTask task1 = new LongRunningTask();

        System.out.println("Before starting task1: " + task1.isAlive());

        task1.start();

        System.out.println("After starting task1: " + task1.isAlive());

        try {
            System.out.println("Main thread waiting for task1 to complete using join()...");
            task1.join();
        } catch (InterruptedException e) {
            System.out.println(e);
        }

        System.out.println("After task1 completion: " + task1.isAlive());
        System.out.println("Main thread continues execution.");
    }
}
```
![output for 7c](https://github.com/yagna123267/JAVALAB-CSE-G/blob/a342a636412c04c52bf84e40841d15315bc2d645/7c%20java.png)
## Title : 8a
```
  class DaemonThread extends Thread {
     public void run() {
      while(true) {
     System.out.println("Daemon thread running");
      try {
      Thread.sleep(500);
       }catch(InterruptedException e) {
        System.out.print(e);
         }
      }
}
}
  class UserThread extends Thread {
     public void run() {
          while(true) {
          for(int i=1;i<=5;i++) {
            System.out.println("User thread iteration:" +i);
            try {  
         Thread.sleep(1000);
          }catch(InterruptedException e) {
             System.out.print(e);
        }
      }
    }
}
}

public class TestDaemon {
    public static void main(String[] args) {
         UserThread  userThread = new UserThread();
        DaemonThread daemonThread = new DaemonThread();
        daemonThread.setDaemon(true);
        userThread.start();
        daemonThread.start();
    }
}
```
## output:
![output for 8a](https://github.com/yagna123267/JAVALAB-CSE-G/blob/2879a526c6f98468a7c920f1410b0f4913563c42/8a%20java.png)
## Title: 8b
```

  class Buffer {
       int[] buffer;
       int count = 0;
       int in = 0, out = 0;
       Buffer(int size) {
         buffer = new int[size];
       }
}
class Consumer {

    int[] buffer;
    int count;
    int out = 0;

    Consumer(int[] buffer, int count) {
        this.buffer = buffer;
        this.count = count;
    }

    synchronized int consume() {
        while (count == 0) {
            try {
                wait();
            } catch (InterruptedException e) {
            }
        }

        int item = buffer[out];
        out = (out + 1) % buffer.length;
        count--;
        notify();
        return item;
    }
}
class Producer {

    int[] buffer;
    int count = 0;
    int in = 0;

    Producer(int size) {
        buffer = new int[size];
    }

    synchronized void produce(int item) {
        while (count == buffer.length) {
            try {
                wait();
            } catch (InterruptedException e) {
            }
        }

        buffer[in] = item;
        in = (in + 1) % buffer.length;
        count++;
        notify();
    }
}
class Producer extends Thread {
    Buffer buffer;

    Producer(Buffer buffer) {
        this.buffer = buffer;
    }

    public void run() {
        for (int i = 1; i <= 10; i++) {
            buffer.produce(i);
            System.out.println("Produced: " + i);
        }
    }
}

  class SharedBuffer {
    int [] buffer;
    int count = 0;
    int in = 0, out = 0;
    Buffer(int size) {
       buffer new int[size];
  class SharedBuffer {
       int[] buffer;
       int count = 0;
       int in = 0, out = 0;
       Buffer(int size) {
         buffer = new int[size];
       }
public class ProducerConsumerDemo {
    public static void main(String[] args) {

        Buffer buffer = new Buffer(5);
        int N = 10;

        Producer p = new Producer(buffer, N);
        Consumer c = new Consumer(buffer, N);

        p.start();
        c.start();
    }
}

```
## output:
![output for 8b](https://github.com/yagna123267/JAVALAB-CSE-G/blob/2879a526c6f98468a7c920f1410b0f4913563c42/8b%20java.png)
## Title: 11
```

class Reservation {
    private int availableBerths;
    Reservation(int berths) {
        this.availableBerths = berths;
    }
    public synchronized void bookTicket(String name, int requestedBerths) {
        System.out.println(name + " is requesting " + requestedBerths + " berths.");
        if (requestedBerths <= availableBerths) {
            System.out.println("Berths available. Booking for " + name);
            availableBerths -= requestedBerths;   
            System.out.println("Ticket booked for " + name);
            System.out.println("Remaining berths: " + availableBerths);
        } else {
            System.out.println("No berths available for " + name);
        }
        System.out.println("--------------------------------");
    }
}
class Person extends Thread {
    private Reservation reservation;
    private String personName;
    private int berthsNeeded;

    // Constructor
    Person(Reservation reservation, String name, int berths) {
        this.reservation = reservation;
        this.personName = name;
        this.berthsNeeded = berths;
    }

    // Step 6: run() method
    public void run() {
        reservation.bookTicket(personName, berthsNeeded);
    }
}
 public class RailwayReservation {
    public static void main(String[] args) {

        // Step 1: Define total available berths
        Reservation reservation = new Reservation(5);

        // Create multiple Person threads
        Person p1 = new Person(reservation, "Ravi", 2);
        Person p2 = new Person(reservation, "Sita", 3);
        Person p3 = new Person(reservation, "Arun", 2);

        // Start threads
        p1.start();
        p2.start();
        p3.start();

   }
}
```
## Output:
![output for](
## Title: addexp 5
```
import java.util.Scanner;
class Cricket {
    String playerName;
    String teamName;
    double battingAverage;
    Cricket(String playerName, String teamName, double battingAverage) {
        this.playerName = playerName;
        this.teamName = teamName;
        this.battingAverage = battingAverage;
    }

    void display() {
        System.out.println("Player: " + playerName + 
                           ", Batting Average: " + battingAverage);
    }
}
  import java.util.Scanner;
public class CricketMain {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        // Input number of players
        System.out.print("Enter number of players: ");
        int n = sc.nextInt();
        sc.nextLine(); // consume newline

        // Declare array
        Cricket[] players = new Cricket[n];

        // Input player details
        for (int i = 0; i < n; i++) {
            System.out.println("\nEnter details for Player " + (i + 1));

            System.out.print("Player Name: ");
}
}
}
```
## Output:
![output for](





























