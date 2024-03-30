## 1.1.3 Describe what happens if you misspell (by, say, omitting the second letter) the following in HelloWorld.java:
    a. public
    b. static
    c. void
    d. args

### a. public

```
HelloWorld.java:1: error: class, interface, enum, or record expected
pblic class HelloWorld {
^
1 error
```

The program won't run and a compiler-time error is displayed informing that a reserved word for type is expected. The error message is not pecise, but can pinpoint where the bug is.

### b. static

```
HelloWorld.java:2: error: <identifier> expected
    public satic void main(String[] args) {
                ^
1 error
```

A compile-time error is displayed informing that a identifier is expected. The error message is precise this time, because the static property is misspelled and the pinpoint is also precise enough.

### c. void

```
HelloWorld.java:2: error: cannot find symbol
    public static vid main(String[] args) {
                  ^
  symbol:   class vid
  location: class HelloWorld
1 error
```

It seems the compiler is seaching for a class vid. It makes sense, since the void represents no return. Altering voit to vit means insted of no return a return of type (class) vid.

### d. args

No error is presented. This fact can be explained by the fact that args is a variable name, consequently there is no probleam in altering its name if all references are altered too.