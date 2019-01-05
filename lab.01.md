# Lab-01

## Goals for this lab

The primary goal of this lab is to help you prepare for the faux lab quiz on Friday. To do this, we'll:
- create a couple of classes on INS using Emacs
- complete a <span>REPL.IT</span> drill together

If you don't know how to get onto INS or into our <span>REPL.IT</span> classroom, then you can pair up with someone else who does. You'll need to get caught up before our quiz on Friday.

---

### INS

Let's create a typical application structure used in this course.

1. Log in to INS.
1. Create a directory called `ins-drill`. 
1. Inside **that** directory, create another directory called `src`.
    - you can do this one of two ways: by using "cd-ing" into `ins-drill` and making the `src` directory, or by using a valid _path_ directly from your home directory
1. cd into the `src` directory and create a Java source file for a class called Drill. The source file doesn't need any "real" content - it just needs to be able to compile without errors.
    - what does the file have to be called?
    - what contents should be in this file?
1. Save your work and then suspend Emacs - don't exit it, because we'll be going back in shortly.
1. Compile your Drill file. You might have some errors; fix them.
1. Once compiled, _predict whether you can run the compiled file._
1. Run the compiled file.
    - Did your prediction come true? If not, why not?
1. Now create a Java source file for a class called Main. Because this will be our entry point into our "application", it needs a proper static main

### <span>REPL.IT</span>

1. Go to our classroom and open `lab 01: our first drill`.
    - Remember: having two classes like this is a bit weird - they're not really in the same file, but the layout here in REPL makes it seem that way.
1. Read the code, _then predict what will happen in the console when the code is run._
1. Run the code.
    - Did your prediction come true? If not, why not?
1. Let's break things in a variety of ways and understand _why_ things are broken. After each mess-up, run the code and read the error messages (as awful as they may look). **Learning to be read and be unafraid of error messages is super-important.**
    - Mess up the spelling of `class` (either one).
    - Change the casing (capitalization) of Main or of UselessMinion.
      - That's odd...refresh the browser and try again.
      - That's even odder, yes? --This is a REPL issue, not a Java issue!--
    - Change the case of System.
    - Change the case of String.
    - Remove a semicolon.
    - Remove a single bracket.
    - Remove a pair of matching brackets (like those after `uselessStatement`).
    - Remove a brace.
1. asd

### ON YOUR OWN

You should now be able to do the `practice lab quiz 00` found in https://github.com/MRU-CSIS-1501-201901-001/lab.quizzes. Make sure you time yourself, as you only have 25 minutes on the real practice quiz Friday.

If you're unable to get through the practice quiz in a timely fashion, practice the areas that are giving you trouble. Don't hesitate to ask for help.
