### 1.1.4 Describe what happens if you put the double quotes in the print statement of HelloWorld.java on different lines, as in this code fragment:
```
System.out.println("Hello,
World");
```

## Answer

```
PrintExperiment.java:3: error: unclosed string literal
        System.out.println("Hello
                           ^
PrintExperiment.java:4: error: unclosed string literal
                            World");
                                 ^
PrintExperiment.java:4: error: not a statement
                            World");
                            ^
3 errors
```

It is displayed multiples errors caused by unclosed string literal.