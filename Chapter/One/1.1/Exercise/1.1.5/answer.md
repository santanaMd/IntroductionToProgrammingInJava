## 1.1.5 Describe what happens if you try to execute UseArgument with each of the following command lines:
    a. java UseArgument java
    b. java UseArgument @!&^%
    c. java UseArgument 1234
    d. java UseArgument.java Bob
    e. java UseArgument Alice Bob

### a. java UseArgument java

```
Hi, java. How are you?
```

Code runs normally.

### b. java UseArgument @!&^%

```
[1] 96346
zsh: ^%: command not found...
Hi, @%. How are you?
[1]  + 96346 done       java UseArgument @%
```

The code is able to run, but with some problems. Part of the non quoted string is interpreted as shell command.

### c. java UseArgument 1234

```
Hi, 1234. How are you?
```

Code runs normally.

### d. java UseArgument.java Bob

```
Hi, Bob. How are you?
```

Code runs normnally.

### e. java UseArgument Alice Bob

```
Hi, Alice. How are you?
```

Code runs normally ignoring the second parameter.
