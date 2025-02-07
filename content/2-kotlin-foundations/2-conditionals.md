# Kotlin Conditionals
Computer programs often operate based on choices. For example, before you came to this page, you were presented with two choices: go to the previous lesson or proceed to this one. You chose to proceed to this one, so the computer program showed you this page. Had you made the opposite decision, you would have been viewing the previous lesson. In a similar way, programs make decisions based on conditions, either from the program itself or user input. This results in customizable outcomes.

## If
The `if` conditional statement executes a block of code if the condition specified is `true`. If the condition is not met, nothing will happen.

```kotlin
if (condition) {
    // Code to execute
}
```

Let's say we want to end a function early if a condition is true.

```kotlin
var keepRunning: Boolean = true

if (!keepRunning) {
    return // This will return from the current function
}

// Code that executes if the program should continue to run
```

## If-Else
The `if-else` statement builds upon the `if` statement. The `if` part works exactly as it does above, but it adds an `else` block, which contains the code that should run if the condition is `false`.

```kotlin
if (condition) {
    // Code to run if condition is true
} else {
    // Code to run if condition is false
}
```

Let's say we want to create a function that takes a grade and returns "Passed" if the grade is greater than or equal to 70, or "Failed" if the grade is less than 70. 
```kotlin
fun evaluateGrade(grade: Int): String {
    return if (grade >= 70) {
        "Passed"
    } else {
        "Failed"
    }
}
```
### Ternary If-Else
Kotlin does not have a traditional ternary operator (condition ? trueValue : falseValue). Instead, it uses the if expression, which works similarly. This is equivalent to the ternary operator in other languages but is more readable and idiomatic in Kotlin.
```kotlin
val result = if (grade >= 70) "Passed" else "Failed"
```

## Else-If
The `else-if` statement builds upon the `if-else` statement. It allows you to check multiple conditions in sequence. If the `if` condition is `false`, the `else-if` conditions are evaluated. If none of the conditions are met, the `else` block is executed.

```kotlin
if (condition1) {
    // Code to run if condition1 is true
} else if (condition2) {
    // Code to run if condition2 is true
} else {
    // Code to run if all conditions are false
}
```

Let's expand our grading function to return a letter grade instead of "Passed" or "Failed".

```kotlin
fun evaluateGrade(grade: Int): String {
    return if (grade >= 90) {
        "A"
    } else if (grade >= 80) {
        "B"
    } else if (grade >= 70) {
        "C"
    } else if (grade >= 60) {
        "D"
    } else if (grade < 60) {
        "F"
    } else {
        "Invalid integer. Must be between 1-100"
    }
}
```

## When Expression
The `when` expression is a powerful alternative to else-if chains. It simplifies complex conditional logic and makes the code more readable and maintainable.
```kotlin
when (variable) {
    value1 -> // Code to run if variable == value1
    value2 -> // Code to run if variable == value2
    else -> // Code to run if no condition is met
}
```

Let's rewrite the grading system using `when`.
```kotlin
fun evaluateGrade(grade: Int): String {
    return when (grade) {
        in 90..100 -> "A"
        in 80..89 -> "B"
        in 70..79 -> "C"
        in 60..69 -> "D"
        in 0..59 -> "F"
        else -> "Invalid integer. Must be between 1-100"
    }
}
```

This produces a much more readable program. Other developers can read this an easily understand how it works and if we want to come back to it to extend it, we can do so easily. 

You can also use `when` without an argument to check multiple conditions.
```kotlin
fun evaluateNumber(number: Int): String {
    return when {
        number > 0 -> "Positive"
        number < 0 -> "Negative"
        else -> "Zero"
    }
}
```

## Exercises
1. Extend the final implementation of the grading function to return more specific letter grades. Instead of just returning broad letter grades like A, B, or C, refine the function to include plus (+) and minus (-) variations, such as A+, A-, B+, B-, and so on. Use this [chart](https://images.squarespace-cdn.com/content/v1/5e1fec6b1e0b0b52a7cb7211/1672926202169-L8FSGEFSNY63L6VVHYJ5/Screen+Shot+2023-01-05+at+7.42.53+AM.png) as reference!
2. A lot of programs have a dedicated administrator account that has total control over a system. 
3. Libraries cannot check out books to cardholders if all copies of the book are already checked out.
## 


