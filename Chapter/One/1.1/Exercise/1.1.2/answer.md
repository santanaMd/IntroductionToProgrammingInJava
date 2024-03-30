## 1.1.2 Describe what happens if you omit the following in HelloWorld.java:
    a. public
    b. static
    c. void
    d. args


## a. public

If the public from class declaration is removed the program can still execute normally, but if the public from the main method declaration is removed the following error is displayed.

```
Error: Main method not found in class HelloWorld, please define the main method as:
   public static void main(String[] args)
or a JavaFX application class must extend javafx.application.Application
```

When the public from class declaration is readded the execution still displays de previous error. We can then assume that not every class must be public or the default permission for a class is public and that every main method must be public.

## b. static

When the reserved word static is removed from the main method declaration the same error presented in the previous item is displayed.

```
Error: Main method not found in class HelloWorld, please define the main method as:
   public static void main(String[] args)
or a JavaFX application class must extend javafx.application.Application
```

Is a valid conclusion to state that, as the reserved word public, the word static is needed to declarate the main method.

## c. void

This time is presented a invalid method declaration error. We can assume that in Java is forbidden to ommit the method's return type.

```
HelloWorld.java:2: error: invalid method declaration; return type required
    public static main(String[] args) {
                  ^
1 error
```

## d. args

One more time the error Main method not found in class is displayed. We can assume that every main method must declare the parameter for line arguments.

```
Error: Main method not found in class HelloWorld, please define the main method as:
   public static void main(String[] args)
or a JavaFX application class must extend javafx.application.Application
```
