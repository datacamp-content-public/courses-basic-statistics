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
ex() %>% check_expr("my_fruit") %>% check_result() %>% check_equal()
success_msg("Nice one! The great advantage of doing calculations with variables is reusability. If you just change my_apples to equal 12 instead of 5 and rerun the script, my_fruit will automatically update as well. Continue to the next exercise.")
```

---

## Back to Apples and Oranges

```yaml
type: NormalExercise
key: 3dc656f752
xp: 100
```

Common sense tells you not to add apples and oranges. The my_apples and my_oranges variables both contained a number in the previous exercise. The + operator works with numeric variables in R. If you really tried to add "apples" and "oranges", and assigned a text value to the variable my_oranges but not to my_apples (see the editor), you would be trying to assign the addition of a numeric and a character variable to the variable my_fruit. This is not possible.

`@instructions`
* Click 'Submit Answer' and read the error message. Make sure to understand why this did not work.
* Adjust the code so that R knows you have 6 oranges and thus a fruit basket with 11 pieces of fruit.

`@hint`
You have to assign the numeric value 6 to the my_oranges variable instead of the character value "six". Note how the quotation marks are used to indicate that "six" is a character.

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# Assign a value to the variable called my_apples
my_apples <- 5 

# Print out the value of my_apples
my_apples       

# Assign a value to the variable my_oranges and print it out
my_oranges <- "six" 
my_oranges 

# New variable that contains the total amount of fruit
my_fruit <- my_apples + my_oranges 
my_fruit
```

`@solution`
```{r}
# Assign a value to the variable called my_apples
my_apples <- 5  

# Print out the value of answer
my_apples  

# Assign a value to the variable my_oranges and print it out
my_oranges <- 6
my_oranges 

# New variable that contains the total amount of fruit
my_fruit <- my_apples + my_oranges 
my_fruit
```

`@sct`
```{r}
ex() %>% check_output("5")
ex() %>% check_output("6")
ex() %>% check_output("11")
success_msg("Awesome, keep up the good work! Continue to the next exercise.")
```

---

## Discover Basic Data Types

```yaml
type: NormalExercise
key: 27c83526fe
xp: 100
```

Some of R's most basic types to get started are:

* Decimals values like 4.5 are called numerics.
* Natural numbers like 4 are called integers. Integers are also numerics.
* Boolean values (TRUE or FALSE) are called logical.
* Text (or string) values are called characters.

Note how the quotation marks on the right indicate that "some text" is a character.

`@instructions`
Change the value of the: - my_numeric variable to 42. - my_character variable to "forty-two". Note that the quotation marks indicate that "forty-two" is a character. - my_logical variable to FALSE.

Note that R is case sensitive!

`@hint`
Replace the values in the editor with the values that are provided in the exercise. 
my_numeric <- 42 assigns the value 42 to the variable my_numeric.

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# What is the answer to the universe?
my_numeric <- 42.5

# The quotation marks indicate that the variable is of type character
my_character <- "some text"

# Change the value of my_logical
my_logical <- TRUE
```

`@solution`
```{r}
# What is the answer to the universe?
my_numeric <- 42

# The quotation marks indicate that the variable is of type character
my_character <- "forty-two"

# Change the value of my_logical
my_logical <- FALSE
```

`@sct`
```{r}
ex() %>% check_output("11")
ex() %>% check_expr("my_character") %>% check_result() %>% check_equal()
ex() %>% check_expr("my_logical") %>% check_result() %>% check_equal()
success_msg("Nice one! The great advantage of doing calculations with variables is reusability. If you just change my_apples to equal 12 instead of 5 and rerun the script, my_fruit will automatically update as well. Continue to the next exercise.")
```

---

## What's that data type?

```yaml
type: MultipleChoiceExercise
key: 8c669e76f6
xp: 50
```

Do you remember that when you added 5 + "six", you got an error due to a mismatch in data types? You can avoid such embarrassing situations by checking the data type of a variable beforehand. You can do this as follows:
```
class(some_variable_name)
```
In the workspace (you can inspect it by typing ls() in the console), some variables have already been defined. Which statement concerning these variables are correct?

`@possible_answers`
* a's class is integer, b is a character, c is a boolean.
* a's class is character, b is a character as well, c is a logical.
* a's class is numeric, b is a string, c is a logical.
* a's class is numeric, b is a character, c is a logical.

`@hint`
You can find out the data type of the a variable for example by typing class(a). You can do similar things for b and c.

`@pre_exercise_code`
```{r}
a <- 42
b <- "forty-two"
c <- 
```

`@sct`
```{r}

```
