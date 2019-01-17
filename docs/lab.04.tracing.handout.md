# Hand Tracing Practice

## CODE BLOCK (I Do)

Trace this code; choose your own values for the keyboard input.

This code has poor naming. On purpose.

You choose what the user enters at the keyboard.

```java

import java.util.Scanner;

public class Main {

  public static void main(String[] args) {
    Scanner kbd = new Scanner(System.in);
    TraceMe trace = new TraceMe();

    int numFargles = kbd.nextInt();
    int numBargles = kbd.nextInt();

    int numArgles = trace.h(numFargles, numBargles);
    System.out.printf("That's %,d argles!%n", numArgles);
  }

}

public class TraceMe {

  public int f(int i, int j) {
    int m = i + j;
    int n = m * 10;

    return n;
  }

  public int g(int a) {
    int b = f(14, a);

    return (b + b) % 9;
  }

  public int h(int x, int y) {
    int z = -f(x / y, y - 1);

    return g(z);
  }

}

```

## CODE BLOCK (We Do)

Trace the code in the static main; choose your own values for the keyboard input.

This code has poor naming. On purpose.

```java

import java.util.Scanner;

public class Main {

  public static void main(String[] args) {
    Scanner kbd = new Scanner(System.in);
    Printatron printatron = new Printatron();

    double n = kbd.nextDouble();

    printatron.printSomething (5.0, n);
    printatron.printSomething ((int)Math.round(n + 0.5));
    printatron.printSomething (n * n, 12.0);
  }

}

public class Printatron {

  public void printSomething (double a, double b) {
    double c = 2 * a + b;
    System.out.println ( a + " " + b + " " + c);
  }
  
  public void printSomething (int a) {
    int x = Math.max(0, a % 2);
    System.out.println ( a + " " + x);
  }

}

```

## CODE BLOCK (You Do)

Trace the code in the static main; choose your own values for the keyboard input.

This code has poor naming. On purpose.

```java

import java.util.Scanner;

public class Trace
{
  public static void main(String args[]) {
    Scanner kbd = new Scanner(System.in);
    int num  = kbd.nextInt();
    int num2 = kbd.nextInt();

    Practice thisIsFun = new Practice();
    num2 = 2 + thisIsFun.f(5);

    System.out.println("Num: " + num);
    System.out.println("Num2: " + num2);
  }
}


public class Practice
{
  public int f(int num) {
    System.out.println("In f ... ");
    num += 5;
    num = h(num);
    g(num);
    System.out.println("... Out F");
    return num;
  }
  
  public void g(int p) {
    int x = h(p) % 5;  
    System.out.print("In G ... ");
    System.out.print(x);
    System.out.println(" ... Out G");
  }
  
  public int h(int num) {
    int x = 5;  
    System.out.print("In H ... ");
    x += num % 4;
    System.out.print(x);
    System.out.println(" ... Out H");
    return x;
  }
}


```