# Hand Tracing Practice

## CODE BLOCK

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

## CODE BLOCK

Trace the code in the static main; choose your own values for the keyboard input.

This code has poor naming. On purpose.

```java

public class Main {

  public static void main(String[] args) {

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