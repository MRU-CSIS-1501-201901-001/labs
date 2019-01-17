# Lab-04

## Goals for this lab

I'm going to admit it - I dropped the ball in explaining tracing in lecture this week. I'm going to rectify that in this lab: I'll do a trace, we'll do a trace together, and then you can do a trace with some of your peers on your own.

---

### INS

Let's create a typical application structure used in this course.

1. Log in to INS.
1. Create a directory called `ins-drill`. 
1. Inside **that** directory, create another directory called `src`.
    - you can do this one of two ways: by  "cd-ing" into `ins-drill` and making the `src` directory, or by using a valid _path_ directly from your home directory
1. cd into the `src` directory and create a Java source file for a class called `Drill`. The source file doesn't need any "real" content - it just needs to be able to compile without errors.
    - what does the file have to be called?
    - what contents should be in this file?
1. Save your work and then suspend Emacs - don't exit it, because we'll be going back in shortly.
1. Compile your Drill file. You might have some errors; fix them.
1. Once compiled, _predict whether you can run the compiled Drill file._
1. Run the compiled file.
    - Did your prediction come true? If not, why not?
1. Now create a Java source file for a class called Main. Because this will be our entry point into our "application", it needs a proper static main.
    - what does **this** file have to be called?
    - what contents should be in **this** file?
1. Save your work and, like before, suspend Emacs.
1. Compile your Main file. You might have some errors; fix them.
1. Once compiled, _predict whether you can run the compiled Main file._
1. Run the compiled file.
    - Did your prediction come true? If not, why not?
1. Add a statement in the static main that creates a new Drill object. Recompile, fix errors, and predict what will happen when we run the compiled Drill file **this** time.
    - Did your prediction come true? If not, why not?
1. Exit any sleeping sessions of Emacs you may have and then log off of INS.

### <span>REPL.IT</span>

1. Go to our classroom and open `lab 01: our first drill`.
    - Remember: having two classes like this is a bit weird - they're not really in the same file, but the layout here in REPL makes it _seem_ that way.
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
1. Let's try and submit the code as-is: click on the `submit` button or hit the drop-down arrow next to `run` and click `run tests`.
    - you should see a disheartening sight: 3 failed tests. Examine the errors. Do they make sense?
    - we want to keep wrasslin' with this, so click on `Keep trying`
1. Let's fix one thing at a time. Let's choose the low-hanging fruit - the method with no inputs: `uselessStatement()`.
1. Next up: `uselessDemand(String thingBeingDemanded)`. This requires us to use **concatenation**.
1. Finally: `uselessSubtractionFact(int a, int b)`. More concatenation here, but we have to be a bit careful....
1. Once we have all 3 "running green" (slang for passing), we can submit...but there's just one thing I'd like to show you first.
    - create a syntax error and rerun the tests...now isn't **that** interesting!
1. That's if for this. Submit your work and call it a day.

### ON YOUR OWN

You should now be able to do the `practice lab quiz 00` found in https://github.com/MRU-CSIS-1501-201901-001/lab.quizzes. Make sure you time yourself, as you only have 25 minutes on the real practice quiz Friday.

If you're unable to get through the practice quiz in a timely fashion, practice the areas that are giving you trouble. Don't hesitate to ask for help.
