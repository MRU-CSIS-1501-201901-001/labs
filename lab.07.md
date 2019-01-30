# Lab-07

## Goals for this lab

- Pick up a few new Emacs commands (useful ones).
- Give you a nudge for the hex grid drill.

---

### NEW EMACS COMMANDS + LINE NUMS

#### LINE NUMBERS

To do this next bit, you need to edit the `.emacs` file that is in your home directory - add the lines shown next to the bottom of the file, and then save your work and exit from Emacs. From that point onward, Emacs will show line numbers!

<pre>
; add line numbers to display
(global-linum-mode 1)
(setq linum-format "%d ")
</pre>

_That "%d " in the last line should look familiar...I wonder if you could tweak it?...._

#### SPLIT SCREEN MODE

I've done this in my screencasts and in lecture...it's pretty darn useful.

> - Ctrl + X, 2 => splits the screen horizontally
> - Ctrl + X, 3 => splits the screen vertically (my fave)
> - Ctrl + X, o => (that's an "oh") go to another pane
> - Ctrl + X, 1 => make the currently selected pane the only one
> - Ctrl + X, 0 => (that's a zero) remove the selected pane
> - Ctrl + X, Ctrl + F => open file in selected pane

#### AUTOCOMPLETE

You can autocomplete what you're typing in Emacs, much like you can autocomplete things you're typing on the command line.

Instead of using `[TAB]`, you use `Alt + /`.

---

### HINT FOR WEEK-03: HEX GRID DRILL

There's a funky thing going on in the method signature here:

```java
  public boolean adjacent(Hex other) {

  }
```

Notice how the type of the sole parameter is `Hex`? That might seem weird to you - you've been used to seeing **primitive types** and **String** in the parameter list up to now. But it's perfectly acceptable - and actually common - to have objects as parameters!

Since the code for `adjacent` is in the `Hex` class itself, **you can talk directly to instance variables of any Hex object**. To do so, you use dot notation, just like we do for methods, but we leave off the brackets.

For example, if you want to "talk" to the `other` parameter in the `adjacent` method, and assuming you have an instance variable in `Hex` called `col`, you could do things like this in your code:

```java
  public boolean adjacent(Hex other) {
    int otherCol = other.col;
  }
```

What's happening here? Well, we have an assignment statement here, right? (See the `=`?) The right-hand side is evaluated first, and it returns whatever value is currently stored in the `other` parameter. Then this value is placed in the local variable `otherCol`. From that point, you can do whatever you want with `otherCol`!
