---
title: 'Intro to basics'
description: ""
free_preview: true
---

## How it works

```yaml
type: NormalExercise
key: 2bafef99a3
lang: r
xp: 100
skills: 1
```

In the editor on the right you should type R code to solve the exercises. When you hit the 'Submit Answer' button, every line of code is interpreted and executed by R and you get a message whether or not your code was correct. The output of your R code is shown in the console in the lower right corner.

R makes use of the # sign to add comments, so that you and others can understand what the R code is about. Just like Twitter! Comments are not run as R code, so they will not influence your result. For example, _Calculate 3 + 4_ in the editor on the right is a comment.

You can also execute R commands straight in the console. This is a good way to experiment with R code, as your submission is not checked for correctness.

`@instructions`
* In the editor on the right there is already some sample code. Can you see which lines are actual R code and which are comments?
* Add a line of code that calculates the sum of 6 and 12, and hit the 'Submit Answer' button.

`@hint`
Just add a line of R code that calculates the sum of 6 and 12, just like the example in the sample code!

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# Calculate 3 + 4
3 + 4

# Calculate 6 + 12

```

`@solution`
```{r}
# Calculate 3 + 4
3 + 4

# Calculate 6 + 12
6 + 12
```

`@sct`
```{r}
ex() %>% check_output("7")
ex() %>% check_output("18")
success_msg("Awesome! Do you see how the console shows the result of the R code you submitted? Now that you're familiar with the interface, let's get down to R business!")
```

---

## Little arithmetics with R

```yaml
type: NormalExercise
key: 3cef4b61e2
xp: 100
```

In its most basic form R can be used as a simple calculator. Consider the following arithmetic operators:

* Addition: +
* Subtraction: -
* Multiplication: *
* Division: /
* Exponentiation: ^
* Modulo: %%
The last three might need some explaining:

* The ^ operator raises the number to its left to the power of the number to its right: for example 3^2 is 9.
* The modulo returns the remainder of the division of the number to the left by the number on its right, for example 5 modulo 3 or 5 %% 3 is 2.
With this knowledge, follow the instructions below to complete the exercise.

`@instructions`
* Type 2^5 in the editor to calculate 2 to the power 5.
* Type 28 %% 6 to calculate 28 modulo 6.
* Click 'Submit Answer' and have a look at the R output in the console.
* Note how the # symbol is used to add comments on the R code.

`@hint`
Another example of the modulo operator: 9 %% 2 equals 1

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# Addition
5 + 5 

# Subtraction
5 - 5 

# Multiplication
3 * 5

 # Division
(5 + 5) / 2 

# Exponentiation


# Modulo

```

`@solution`
```{r}
# Addition
5 + 5 

# Subtraction
5 - 5 

# Multiplication
3 * 5

 # Division
(5 + 5) / 2 

# Exponentiation
2 ^ 5

# Modulo
28 %% 6
```

`@sct`
```{r}
ex() %>% check_output("10")
ex() %>% check_output("0")
ex() %>% check_output("15")
ex() %>% check_output("5")
ex() %>% check_output("32")
ex() %>% check_output("4")
success_msg("Great! Head over to the next exercise.")
```

---

## Documenting your code

```yaml
type: NormalExercise
key: 0e8458804e
xp: 100
```

Adding comments to your code is extremely important to make sure that you and others can understand what your code is about. R makes use of the # sign to add comments.

It's important to note that comments are not run as R code, so they will not influence your result. For example, Calculate 3 + 4 in the editor on the right is a comment and is ignored during execution.



`@instructions`
Add another comment in the editor on the right, Calculate 6 + 12, at the appropriate location.

`@hint`
Simply add the line # Calculate 6 + 12 above the R code that calculates 6 + 12.

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# Calculate 3 + 4
3 + 4


6 + 12
```

`@solution`
```{r}
# Calculate 3 + 4
3 + 4

# Calculate 6 + 12
6 + 12
```

`@sct`
```{r}
ex() %>% check_code()
success_msg("Great! Looks better, doesn't it? Proceed to the next exercise.")
```

---

## Variable assignment I

```yaml
type: NormalExercise
key: 89f3af7de9
xp: 100
```

A basic concept in R programming is the **variable**. It allows you to store a value or an object in R. You can then later use this variable's name to easily access the value or the object that is stored within this variable. You use <- to assign a variable:
```
my_variable <- 4
```

`@instructions`
Complete the code in the editor such that it assigns the value 42 to the variable `x` in the editor. Click 'Submit Answer'. Notice that when you ask R to print `x`, the value 42 appears.

`@hint`
Look at how the value 4 was assigned to my_variable in the exercise's assignment. Do the exact same thing in the editor, but now assign 42 to the variable x.

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# Assign the value 42 to x
x <- 

# Print out the value of the variable x
x
```

`@solution`
```{r}
# Assign the value 42 to x
x <- 42

# Print out the value of the variable x
x
```

`@sct`
```{r}
ex() %>% check_output("42")
success_msg("Good job! Notice that R does not print the value of a variable to the console when you do the assignment. x <- 42 did not generate any output, because R assumes that you will be needing this variable in the future. Otherwise you wouldn't have stored the value in a variable in the first place, right? Proceed to the next exercise!")
```

---

## Variable assignment II

```yaml
type: NormalExercise
key: 529be8098e
xp: 100
```

Variables are great to perform arithmetic operations with. In this assignment, we have defined a variable my_apples. You want to define another variable called my_oranges and add these two together.

```
my_apples + my_oranges
```

`@instructions`
* Create a variable called my_oranges and assign it the value of 6.
* Add the variables my_apples and my_oranges and have R simply print the result.
* Combine the variables my_apples and my_oranges into a new variable my_fruit, which is the total amount of fruits in your fruit basket.

`@hint`
my_fruit is just the sum of my_apples and my_oranges. You can use the + operator to sum the two and <- to assign that value to the variable my_fruit.

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# Assign a value to the variables my_apples and my_oranges
my_apples <- 5


# Add these two variables together and print the result


# Create the variable my_fruit

```

`@solution`
```{r}
# Assign a value to the variables my_apples and my_oranges
my_apples  <- 5
my_oranges <- 6

# Add these two variables together and print the result
my_apples + my_oranges

# Create the variable my_fruit
my_fruit <- my_apples + my_oranges
```

`@sct`
```{r}
ex() %>% check_output("11")
ex() %>% check_that(is_true(my_fruit == 11))
success_msg("Nice one! The great advantage of doing calculations with variables is reusability. If you just change my_apples to equal 12 instead of 5 and rerun the script, my_fruit will automatically update as well. Continue to the next exercise.")
```
