# Lab-11

## Goals for this lab

We'll look at how you can compile **inside** of Emacs and jump to errors easily.
Then I'll talk about how you can actually read the test code in A1 to help you figure out your problems.

### COMPILING in EMACS

Yes, it's true: you **can** compile from the comfort and safety of your own Emacs window!

> `Alt + X, compile` will javac the current file
> ``Ctrl + X, ` `` (that's the backtick - under the Esc key) will jump to the next error in your code

This can be a super-efficient way to burn through your errors....use it.

### READING TEST CODE for ASSIGNMENTS

So you know that `tests` directory that's been in the quizzes and is in asg.01? Therein lies the code that tests your code.

It can be super-helpful to take a peek in there.

For example, in `tests\JudoMatchTests.java`:

```Java
    @Test
    @DisplayName("game should be over if blue scores an awasete ippon")
    public void game_over_if_blue_awasete_ippon()  {
        judoMatch.process("10 b w");
        judoMatch.process("10 b w");
        assertThat(judoMatch.over()).isTrue();
    }
```

So what's going on here? Well...

- the `@Tests` marks the block of code as a runnable test
- the `@DisplayName` determines what prints out when the test is run
- the body of the method is what we're _really_ interested in, though. For _this_ test:
   - a judo match is told to process "10 b w"
   - it's told to do that again
   - the next part (`assertThat`) is saying "pass the test if `judoMatch.over()` returns a value of true"

Here's a slightly different test in the same file:

```Java
 @Test
    @DisplayName("blue wins by awasete ippon")
    public void blue_wins_by_awasete_ippon()  {
        judoMatch.process("14 b w");
        judoMatch.process("14 b w");

        assertThat(judoMatch.winner()).isEqualTo("blue");
    }
```

In this one, we're confirming that after the two "14 b w" events are processed, the method `judoMatch.winner()` should return the string `"blue"`