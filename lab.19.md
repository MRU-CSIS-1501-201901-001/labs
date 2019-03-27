# Lab-19

## Goals for this lab

Let's play with file reading a bit in a lab setting. Coding this stuff is different than reading about it, or working on a blackboard.

### LET'S DO ONE TOGETHER

_(Though it would be **_easier_** to do the following in a REPL, we'll instead do it on INS, since that's where your assignment will be done.)_

Let's code up a class that reads in a text file and has these public methods that provide basic information about the file contents.

```Java
// constructor
public TextFileAnalyzer(String path) throws FileNotFoundException

// returns number of lines in the file
public int numLines()

// returns the number of characters in the file
public int numChars()

//returns the number of words in the file
public int numWords()
```

### NOW YOU DO ONE

Next, it's your turn. Code up a class called UserLoader that loads user data from a file consisting of a usernames and ages; you'll return these as an ArrayList<User>. Yes, that means you have another class to make!

Here's the public API you should have for the (non-User) class:

```Java
// constructor
public UserLoader(String path) throws FileNotFoundException

// returns number of User's loaded
public int numUsers()

// returns Users in the given file
public ArrayList<User> loadedUsers()
```

### SO...ASG.03

You should now have enough experience to get a start on the `load()` method in the `HighScorePersistenator` class in asg.03. 

If you don't yet have a HighScores class completed - and it's no biggie if that's the case - then have `load()` return null and print out what's being read to the console. At least it's a start!
