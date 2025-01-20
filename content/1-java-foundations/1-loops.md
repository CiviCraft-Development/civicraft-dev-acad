# Loops
Loops allow a block of code to be repeatedly executed as long as a specified condition is met. Each type of loop serves a unique purpose and is used in different scenarios.

## For Loop
For loops are used when the number of iterations is known beforehand. The loop executes the code within its block until the condition defined in the for loop is met.

```java
for (initialization; condition; increment) {
    // Code to execute
}
```
A for loop consists of three main components inside the parentheses:
1. **Initialization**: A variable is declared and initialized. This variable is typically used in the loop's condition and increment.
2. **Condition**: The loop will continue to execute as long as this condition evaluates to true.
3. **Increment/Decrement**: This updates the loop variable after each iteration.

```java
for (int i = 1; i <= 10; i++) {
    System.out.println(i);
}
```
In this example, the loop starts with the integer `i` initialized to 1. The loop continues running as long as `i` is less than or equal to 10. The increment `i++` increases the value of `i` by 1 after each iteration. The loop prints numbers from 1 to 10, each on a new line.

## For-Each Loop / Enhanced For Loop
For-each loops, also known as enhanced for loops, are used to iterate over each element in a collection, such as an array or list, and perform an action on or with each element.

```java
for (dataType variable : collection) {
    // Code to execute
}
```

The first part declares a variable to represent each individual element of the collection, while the second part specifies the collection to iterate over. The loop automatically iterates through all elements of the collection without needing a condition or increment.

```java
int arr[] = {1, 2, 3, 4, 5};

for (int i : arr) {
    System.out.println(i + 10);
}
```
In this example, the array `arr` contains integers from 1 to 5. The for-each loop declares an integer `i` that represents each element of the array in sequence. The loop adds 10 to each element and prints the result, producing numbers 11 to 15, each on a new line. This approach is efficient for iterating through collections without manually managing indexes.

## While Loop
While loops are used when the end condition is not known in advance or depends on a condition that may change dynamically during execution. The loop checks the condition before executing the code block, and the code is only executed if the condition evaluates to true. 

```java
while (condition) {
    // Code to execute
}
```
The condition is evaluated before each iteration. If the condition is true, the code inside the loop executes. If the condition is false initially, the loop does not run at all. Care must be taken to update variables within the loop to ensure the condition can eventually evaluate to false, preventing infinite loops.

```java
int i = 1;
while (i < 10) {
    System.out.println(i);
    i++;
}
```
In this example, the loop starts with the integer `i` initialized to 1. The condition `i < 10` ensures the loop will execute as long as `i` is less than 10. On each iteration, `i` is printed and incremented by 1. The loop terminates when `i` reaches 10, producing an output of numbers from 1 to 9, each on a new line.

## Do-While Loop
Do-while loops are similar to while loops but differ in one key way: the code block is executed first, and the condition is checked afterward. This ensures that the code within the loop runs at least once, regardless of whether the condition is true.

```java
do {
    // Code to execute
} while (condition);
```

The condition is evaluated after the code block is executed. If the condition is true, the loop continues to execute. If the condition is false, the loop terminates after the first execution.

```java
int i = 1;
do {
    System.out.println(i);
    i++;
} while (i < 10);
```

In this example, the integer `i` is initialized to 1. The code inside the do block executes first, printing `i` and incrementing it by 1. Then the condition `i < 10` is evaluated. The loop continues as long as the condition remains true. Even if `i` were initially greater than or equal to 10, the code block would still execute once, guaranteeing at least one output. In this case, the output is numbers from 1 to 9, each on a new line.
