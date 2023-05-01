# While Loops In Java
Loops are used in programming to repeat the execution of code instead of writing the line code of over and over again.

## A Code Example
```java
int countdown = 5; 
while (countdown >= 0) {
    System.out.println(countdown);
    countdown--;
}
```
## Line by Line Analysis

```java
int countdown = 5
```
> We have set an outer variable to help us with our while loop.

```java
while (countdown >= 0)
```
> While is a keyword in java.
>
> It helps us start a looping structure.
>
> Much like an _if statement_ a while loop will execute its code block when its _boolean expression_ is true.
>
> Unlike an if statement, _a while loop will continue to execute its code block_ as long as the __boolean expression is true__.

```java
countdown--;
```
> This line of code just decrements countdown variable by 1 at every iteration.

## Formalization

__Iterations__: instructions or code being repeated until a specific end result is achieved.

__While Loop Format in Java__:
```java
while (condition) {
    // code to be executed repeatedly
}
```

__Infinite Loop:__ An infinite loop is a while loop that never ends because the boolean condition of the loop never turns to false.

_Example:_
```java
String value = "Hello";
while (value.equals("Hello")) {
    System.out.println("Hello");
}
```

## Using While Loops as a Counter
```java
int counter = 0;
while (counter <= 10) {
    System.out.println("The counter is at: " + counter);
    counter++; // Incremental operator to increase a variable by 1.
}
```

By using some sort of a counting variable, you get to control the number of iterations you execute.

## Using a boolean variable to control when to end a while loop
```java
String user_input;
boolean loop = true;

while (loop == true) {
    System.out.println("Hello, World!");

    // Loop exiting code
    System.out.println("Would you like to end the loop? (Yes/No).");
    user_input = in.nextLine();
    if (user_input.equals("Yes")) {
        loop = False;
    }
}
```

We can also take an user input every iteration to check if they want to exit to prevent an infinite loop.