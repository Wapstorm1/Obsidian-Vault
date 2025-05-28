- A **method** in Java is a block of code that performs a specific task. You can think of it as a **function** that you can call whenever you need to reuse the same logic.
```
public static int addNumbers(int a, int b) {

        return a + b; // Returns the sum

```


- A **class** is like a **blueprint** or **template**. It defines the structure and behavior (variables and methods) of an object.

```
class Car {

    String color; // Variable (property)

    int speed;    // Variable (property)

    void drive() { // Method (behavior)

        System.out.println("The car is driving.");

    }

}

```


- An **object** is a **real instance** of a class. If a class is a blueprint, an object is the actual house built from that blueprint. Each object has its own **data** and can perform actions defined in the class.

```
public class Main {

    public static void main(String[] args) {

        Car myCar = new Car(); // Create an object of the Car class

        myCar.color = "Red";   // Set the color property

        myCar.speed = 100;     // Set the speed property

        myCar.drive();         // Call the drive method

        System.out.println("My car color is: " + myCar.color); // Output: Red

    }
}
```







- In Java you need to declare a data type for a variable
```
for (String s: name){} - Enhanced array of strings

break; - stop anything from executing
for (int i = array.length - 1; i >= 0; i--){} - reverse order of an array

for (String val :a) {} - enhanced size array
a.contains(String) - check the value in the array

List<String> newName = Arrays.asList(originalArray);
charAt(i) - to get string letter by letter
```
- In Java ==String== is an ==object== that represents the sequense of the characters. THere are 2 ways of representing string: string leteral and allocating new object. ![[Pasted image 20241101185524.png]]
![[Pasted image 20241101190217.png]]
- **Streams**
  Streams in Java are a tool for processing data in a clean and efficient way. Think of them as pipelines where data flows through a series of operations like filtering, transforming, and collecting.
  ![[Pasted image 20241119165948.png]]

- When you use variable in a loop it stores during the loop execution. 

```
public class Bottles {


public static void main(String[] args) {

int x = 0;

while(x < 4) {

System.out.print("a");

if(x < 1) {

System.out.print(" ");

}

System.out.print("n");

if( x > 1) {

System.out.print(" oyster ");

x = x + 2;

}

  

if (x==1) {

System.out.print("noys");

  

}

if(x<1) {

System.out.print("oise ");

  

}

System.out.println();

x = x +1;

}

}

}
```


![[Pasted image 20241219203610.png]]

