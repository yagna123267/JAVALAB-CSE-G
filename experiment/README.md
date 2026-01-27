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
``
## output:
![output for multilevel inheritance](https://github.com/yagna123267/JAVALAB-CSE-G/blob/5afb7ac166f21979094faa4a93d81178cbd56c7c/experiment/4b.output.png)
































