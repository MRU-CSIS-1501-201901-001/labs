# Lab-08

## Goals for this lab

- Pick up a few debugging pointers.
- Take a look at the assignment.

---

## DEBUGGING TIPS

### GET TO KNOW COMMON ERRORS

Although you'll see a lot of different kinds of compile time errors during this course (and onward, perhaps?), some are more common than others.

Here is a useful guide to some of the more common ones: http://www.terryanderson.ca/debugging/compile.html

### GENERAL STRATEGIES WHEN FACED WITH ERRORS

- always start with the first error; don't cherry pick ones that seem "easier", because often fixing the first error will fix some (or all!) of the following errors!
- **read** the entire error message, not just the line number (though that's important!), since it will often give you useful information
- use System.out.println to print out the values of variables in sections of code that you suspect might be broken; these kind of prints have a special name: **trace statements** - and they're **very** useful.
  - if you give each of your classes a useful `toString` that displays instance variable information, trace statements become even **more** useful!
- start looking for errors on the line of code that prints out the thing you don't like; that line will often lead you to another line, which leads to another...which will almost always lead you back to the root cause of your problem

### STACK TRACES

StackTraceExampleTwo.java
StackTraceExampleOne.java

---

## ASSIGNMENT 1 INTRO

Take a look over the documentation - there's a lot there, but it's all there for a reason!

Make sure you understand what you're being asked to build before you start doing ANY coding: if you don't have a clear goal in mind, there's no possible way you can succeed!
