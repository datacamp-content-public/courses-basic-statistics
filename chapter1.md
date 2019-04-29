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

Adding comments to your code is extremely important to make sure that you and others can understand what your code is about. R makes use of the `#` sign to add comments.

It's important to note that comments are not run as R code, so they will not influence your result. For example, _Calculate 3 + 4_ in the editor on the right is a comment and is ignored during execution.

`@instructions`
Add another comment in the editor on the right, _Calculate 6 + 12_, at the appropriate location.

`@hint`
Simply add the line `# Calculate 6 + 12` above the R code that calculates 6 + 12.

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
Look at how the value 4 was assigned to my_variable in the exercise assignment. Do the exact same thing in the editor, but now assign 42 to the variable x.

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
* a 's class is integer, b is a character, c is a boolean.
* a 's class is character, b is a character as well, c is a logical.
* a 's class is numeric, b is a string, c is a logical.
* a 's class is numeric, b is a character, c is a logical.

`@hint`
You can find out the data type of the a variable for example by typing class(a). You can do similar things for b and c.

`@pre_exercise_code`
```{r}
a <- 42
b <- "forty-two"
c <- FALSE
```

`@sct`
```{r}
msg1 <- "Not good, try again!"
msg2 <- "Not good, try again!"
msg3 <- "Not quite, give it another shot."
msg4 <- "Nice one. Let's step it up a notch and start coercing variables!"
ex() %>% check_mc(4, feedback_msgs = c(msg1, msg2, msg3, msg4))
```

---

## Coercion: Taming your data

```yaml
type: NormalExercise
key: 3b3c8f7d1b
xp: 100
```

It is possible to transform your data from one type to the other. Next to the class() function, you can use the as.*() functions to enforce data to change types. For example,

```
var <- "3"
var_num <- as.numeric(var)
```
converts the character string "3" in var to a numeric 3 and assigns it to var_num. However, keep in my that it is not always possible to convert the types without losing information or getting errors.

```
as.integer("4.5")
as.numeric("three")
```
The first line will convert the character string "4.5" to the integer 4. The second one will convert the character string "three" to an NA.

`@instructions`
* var1 is logical. Convert it to character and assign it to the variable var1_char.
* Next, see whether var1_char actually is a character by using the is.character() function on it.
* var2 is numeric. Convert it logical and assign it to the variable var2_log.
* Inspect the class of var2_log using class(). And, finally, var3 is of type character. Convert it to numeric and assign the result to var3_num. Was it successful?

`@hint`


`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# Create variables var1, var2 and var3
var1 <- TRUE
var2 <- 0.3
var3 <- "i"

# var1 is logical; convert it to character: var1_char

# See whether var1_char is a character

# var2 is numeric; convert it to logical: var2_log

# Inspect the class of var2_log

# var3 is character; convert it to numeric: var3_num  
```

`@solution`
```{r}
# Create variables var1, var2 and var3
var1 <- TRUE
var2 <- 0.3
var3 <- "i"

# Convert var1 to a character: var1_char
var1_char <- as.character(var1)
# See whether var1_char is a character
is.character(var1_char)
# Convert var2 to a logical: var2_log
var2_log <- as.logical(var2)
# Inspect the class of var2_log
class(var2_log)
# Coerce var3 to a numeric: var3_num
var3_num <- as.numeric(var3)
```

`@sct`
```{r}
ex() %>% check_expr("var1_char") %>% check_result() %>% check_equal()
ex() %>% check_expr("var2_log") %>% check_result() %>% check_equal()
ex() %>% check_output_expr("class(var2_log)")
ex() %>% check_expr("var3_num") %>% check_result() %>% check_equal()
success_msg("Well done, this concludes the exercises of working with variables")
```

---

## Create a vector I

```yaml
type: NormalExercise
key: 485cfb9cb3
xp: 100
```

On your way from rags to riches, you will make extensive use of vectors. Vectors are one-dimension arrays that can hold numeric data, character data, or logical data. In other words, a vector is a simple tool to store data. For example, you can store your daily gains and losses in the casinos.

In R, you create a vector with the combine function c(). You place the vector elements separated by a comma between the brackets. For example:

```
numeric_vector <- c(1, 2, 3)
character_vector <- c("a", "b", "c")
boolean_vector <- c(TRUE, FALSE)
```

Once you have created these vectors in R, you can use them to do calculations.

`@instructions`
Complete the code such that boolean_vector contains the three elements: TRUE, FALSE and TRUE (in that order).

`@hint`
Assign c(TRUE,FALSE,TRUE) to the variable boolean_vector with the <- operator. You can also use the shorter notations, T and F for TRUE and FALSE respectively.

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
numeric_vector <- c(1, 10, 49)
character_vector <- c("a", "b", "c")

# Complete the code for 'boolean_vector'

```

`@solution`
```{r}
numeric_vector <- c(1, 10, 49)
character_vector <- c("a", "b", "c")

# Complete the code for 'boolean_vector'
boolean_vector <- c(TRUE, FALSE, TRUE)
```

`@sct`
```{r}
ex() %>% check_expr("boolean_vector") %>% check_result() %>% check_equal()
success_msg("Awesome! You defined one great boolean vector!")
```

---

## Vectors II

```yaml
type: NormalExercise
key: 4ace475364
xp: 100
```

In the previous assignment, you created 3 vectors: a numeric vector, a character vector and a boolean vector. Sometimes you only want to select a specific element from one of those vectors instead of using the entire vector. R makes this very easy using indexing.

Indexing entails the use of square brackets [] to select elements from a vector. For instance, `numeric_vector[1]` will select the first element of the vector `numeric_vector`. `numeric_vector[c(1,3)]` will select the first and the third element of the vector numeric_vector.

`@instructions`
* Select the letter "a" from character_vector
* Select the second and the third element of boolean_vector

`@hint`
a is the first element of character_vector and can thus be selected using character_vector[1].

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# A numeric vector containing 3 elements
numeric_vector <- c(1, 10, 49)

# a character vector containing 3 elements
character_vector <- c("a", "b", "c")

# Complete the code for 'boolean_vector'
boolean_vector <- c(TRUE, FALSE, TRUE)
```

`@solution`
```{r}
# A numeric vector containing 3 elements
numeric_vector <- c(1, 10, 49)

# a character vector containing 3 elements
character_vector <- c("a", "b", "c")

# Complete the code for 'boolean_vector'
boolean_vector <- c(TRUE, FALSE, TRUE)

# select the letter a from character vector
character_vector[1]

# select the second and third element of the vector boolean vector
boolean_vector[c(2,3)]
```

`@sct`
```{r}
ex() %>% check_output_expr("character_vector[1]")
ex() %>% check_output_expr("boolean_vector[c(2,3)]")
success_msg("Well done!")
```

---

## Selection by comparison I

```yaml
type: NormalExercise
key: ed5c8e866b
xp: 100
```

Sometimes you want to select elements from a vector in a more advanced fashion. This is where the use of logical operators may come in handy.

The (logical) comparison operators known to R are: - < for less than - > for greater than - <= for less than or equal to - >= for greater than or equal to - == for equal to each other - != not equal to each other

The nice thing about R is that you can use these comparison operators on vectors. For example, the statement c(4,5,6) > 5 returns: FALSE FALSE TRUE. In other words, you test for every element of the vector if the condition stated by the comparison operator is TRUE or FALSE.


`@instructions`
* Behind the scenes, R does an element-wise comparison of each element in the vector c(4,5,6) with the element 5. However, 5 is not a vector of length three. To solve this, R automatically replicates the value 5 to generate a vector of three elements, c(5, 5, 5) and then carries out the element-wise comparison.

* Check which values in numeric_vector are larger than 10. Assign the result to the variable larger_than_ten.
* print the variable larger_than_ten to the console.

`@hint`
Use the operator the following code to get values larger than 10: numeric_vector > 10

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# A numeric vector containing 3 elements
numeric_vector <- c(1, 10, 49)

```

`@solution`
```{r}
numeric_vector <- c(1, 10, 49)
larger_than_ten <- numeric_vector > 10
larger_than_ten
```

`@sct`
```{r}
ex() %>% check_output_expr("larger_than_ten")
ex() %>% check_expr("larger_than_ten") %>% check_result() %>% check_equal()
success_msg("Well done!")
```

---

## Selection by comparison II

```yaml
type: NormalExercise
key: 10e19fc07c
xp: 100
```

In the last exercise we saw larger_than_ten consisted of a vector of TRUE and FALSE. We make use of this logical vector to select elements from another vector. For instance, `numeric_vector[c(TRUE, FALSE, TRUE)]` will select the first and the third element from the vector numeric_vector.

`@instructions`
Print the items from numeric_vector that are larger than 10

`@hint`
You may want to use the vector larger_than_ten for indexing the vector numeric_vector.

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
numeric_vector <- c(1, 10, 49)
larger_than_ten <- numeric_vector > 10
```

`@solution`
```{r}
numeric_vector <- c(1, 10, 49)
larger_than_ten <- numeric_vector > 10
numeric_vector[larger_than_ten]
```

`@sct`
```{r}
ex() %>% check_output_expr("numeric_vector[larger_than_ten]")
success_msg("Great job, you seem to get indexing!")
```

---

## Matrices

```yaml
type: NormalExercise
key: 2e75875c91
xp: 100
```

In R, a matrix is a collection of elements of the same data type (numeric, character, or logical) arranged into a fixed number of rows and columns. Since you are only working with rows and columns, a matrix is called two-dimensional.

You can construct a matrix in R with the matrix() function. Consider the following example: 
```
matrix(1:9, byrow = TRUE, nrow = 3, ncol = 3)
```
In the matrix() function:

* The first argument is the collection of elements that R will arrange into the rows and columns of the matrix. Here, we use 1:9 which constructs the vector c(1, 2, 3, 4, 5, 6, 7, 8, 9).
* The argument byrow indicates that the matrix is filled by the rows. 
* The third argument nrow - three rows.
* The fourth argument ncol indicates the number of columns that the matrix should have


`@instructions`
* Construct a matrix with 5 rows and 4 columns containing the numbers 1 up to 20 and assign it to the variable m. Specify the byrow argument to be TRUE
* Print m to the console

`@hint`
You may want to try something like 
```
matrix(data, byrow = TRUE, nrow = 5, ncol = 4)
```

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# Construction of a matrix with 5 rows that contain the numbers 1 up to 20 and assign it to m


# print m to the console
```

`@solution`
```{r}
# Construction of a matrix with 5 rows that contain the numbers 1 up to 20
m <- matrix(1:20, byrow = TRUE, nrow = 5, ncol = 4)
m
```

`@sct`
```{r}
ex() %>% check_output_expr("m")
ex() %>% check_expr("m") %>% check_result() %>% check_equal()
success_msg("Great job, you can now create matrices!")
```

---

## Factors

```yaml
type: NormalExercise
key: 32a00ec357
xp: 100
```

In this exercise you dive into the wonderful world of factors.

The term factor refers to a statistical data type used to store categorical variables. The difference between a categorical variable and a continuous variable is that a categorical variable can belong to a limited number of categories. A continuous variable, on the other hand, can correspond to an infinite number of values.

It is important that R knows whether it is dealing with a continuous or a categorical variable, as the statistical models you will develop in the future treat both types differently.

`@instructions`
* A good example of a categorical variable is the variable `student_status`. An individual can either be "student" or "not student". This means that "student" and "not student" are two values of the categorical variable `student_status` and every observation can be assigned one of these values. We can do this using the `factor` function.

* Turn the vector student_status into a factor and put this in a variable called categorical_student
* Print the variable categorical_student

`@hint`
You may want to try `factor(student_status)` and store this in the variable `categorical_student`

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# a vector called student_status
student_status <- c("student", "not student", "student", "not student")

# turn student_status into a factor and save it in the variable categorical_student


# print categorical_student to the console
```

`@solution`
```{r}
# a vector called student_status
student_status <- c("student", "not student", "student", "not student")
categorical_student <- factor(student_status)
categorical_student
```

`@sct`
```{r}
ex() %>% check_output_expr("categorical_student")
ex() %>% check_expr("categorical_student") %>% check_result() %>% check_equal()
success_msg("Great job, you can now construct factors!")
```

---

## Dataframes: What's a data frame?

```yaml
type: NormalExercise
key: 3b7801f987
xp: 100
```

You may remember the matrix, a multi-dimensional object that we discussed earlier. All the elements that you put in a matrix should be of the same type. However, when performing a market research survey, you often have questions such as:

* 'Are your married?' or 'yes/no' questions (= boolean data type)
* 'How old are you?' (= numeric data type)
* 'What is your opinion on this product?' or other 'open-ended' questions (= character data type)


`@instructions`
The output, namely the respondents' answers to the questions formulated above, is a data set of different data types. You will often find yourself working with data sets that contain different data types instead of only one. A data frame has the variables of a data set as columns and the observations as rows. This will be a familiar concept for those coming from different statistical software packages such as SAS or SPSS.

* print the object mtcars to the console.

`@hint`
All you need to do is type "mtcars" in your script

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# print mtcars to the console
```

`@solution`
```{r}
# solution code
mtcars
```

`@sct`
```{r}
ex() %>% check_output_expr("mtcars")
ex() %>% check_expr("mtcars") %>% check_result() %>% check_equal()
success_msg("You just printed your first dataframe")
```

---

## Inspecting dataframes

```yaml
type: NormalExercise
key: 70855f1cb0
xp: 100
```

There are several functions you can use to inspect your dataframe. To name a few

* head: this by default prints the first 6 rows of the dataframe
* tail: this by default prints the last 6 rows to the console
* str: this prints the structure of your dataframe
* dim: this by default prints the dimensions, that is, the number of rows and columns of your dataframe
* colnames: this prints the names of the columns of your dataframe

`@instructions`
* Print the first 6 rows of mtcars
* Print the structure of the dataframe mtcars
* Print the dimensions of the dataframe mtcars

`@hint`
Think about the functions head, str and dim.

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# print the first 6 rows of mtcars


# print the structure of mtcars


# print the dimensions of mtcars


```

`@solution`
```{r}
# print the first 6 rows of mtcars
head(mtcars)

# print the structure of mtcars
str(mtcars)

# print the dimensions of mtcars
dim(mtcars)
```

`@sct`
```{r}
ex() %>% check_output_expr("head(mtcars)")
ex() %>% check_output_expr("str(mtcars)")
ex() %>% check_output_expr("dim(mtcars)")
success_msg("Good job, you'll become an expert in looking at your data")
```

---

## Constructing a dataframe yourself

```yaml
type: NormalExercise
key: cb326419c3
xp: 100
```

Since using built-in data sets is not even half the fun of creating your own data sets, the rest of this chapter is based on your personally developed data set.

As a first goal, you want to construct a data frame that describes the main characteristics of eight planets in our solar system. The main features of a planet are:

* The type of planet (Terrestrial or Gas Giant).
* The planet's diameter relative to the diameter of the Earth.
* The planet's rotation across the sun relative to that of the Earth.
* If the planet has rings or not (TRUE or FALSE).


`@instructions`
You construct a data frame with the data.frame() function. As arguments, you should provide the above mentioned vectors as input that should become the different columns of that data frame. Therefore, it is important that each vector used to construct a data frame has an equal length. But do not forget that it is possible (and likely) that they contain different types of data.

* Use the function data.frame() to construct a data frame. Call this variable planet_df.

`@hint`
You can wrap each individual vector in the data.frame() function separated by a comma

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# planets vector
planets <- c("Mercury", "Venus", "Earth", "Mars", "Jupiter", "Saturn", "Uranus", "Neptune")

# type vector
type <- c("Terrestrial planet", "Terrestrial planet", "Terrestrial planet", "Terrestrial planet", "Gas giant", "Gas giant", "Gas giant", "Gas giant")
# diameter vector
diameter <- c(0.382, 0.949, 1, 0.532, 11.209, 9.449, 4.007, 3.883)
# rotation vector
rotation <- c(58.64, -243.02, 1, 1.03, 0.41, 0.43, -0.72, 0.67)
# rings vector
rings <- c(FALSE, FALSE, FALSE, FALSE, TRUE, TRUE, TRUE, TRUE)

# construct a dataframe planet_df from all the above variables
```

`@solution`
```{r}
# planets vector
planets <- c("Mercury", "Venus", "Earth", "Mars", "Jupiter", "Saturn", "Uranus", "Neptune")

# type vector
type <- c("Terrestrial planet", "Terrestrial planet", "Terrestrial planet", "Terrestrial planet", "Gas giant", "Gas giant", "Gas giant", "Gas giant")
# diameter vector
diameter <- c(0.382, 0.949, 1, 0.532, 11.209, 9.449, 4.007, 3.883)
# rotation vector
rotation <- c(58.64, -243.02, 1, 1.03, 0.41, 0.43, -0.72, 0.67)
# rings vector
rings <- c(FALSE, FALSE, FALSE, FALSE, TRUE, TRUE, TRUE, TRUE)

# construct a dataframe planet_df from all the above variables
planet_df <- data.frame(planets, type, diameter, rotation, rings)
```

`@sct`
```{r}
ex() %>% check_expr("planet_df") %>% check_result() %>% check_equal()
success_msg("Good job, you'll become an expert with data frames")
```

---

## Indexing and selecting columns from a dataframe

```yaml
type: NormalExercise
key: d1fcbba5cb
xp: 100
```

In the same way as you indexed your vectors, you can select elements from your dataframe using square brackets. Different from dataframes however, you now have multiple dimensions: rows and columns. That's why you can use a comma in the middle of the brackets to differentiate between rows and columns. For instance, the following code `planet_df[1,2]` would select the element in the first row and the second column from the dataframe planet_df.

You can also use the $ operator to select an entire column from a dataframe. For instance, planet_df$planets would select the entire planets column from the dataframe planet_df.

`@instructions`
* Select the elements in the first row, and the second and third column from planet_df
* Select the entire third column from planet_df

`@hint`
Remember how you could use the c operator: `planet_df[1, c(2,3)]`

`@pre_exercise_code`
```{r}
# planets vector
planets <- c("Mercury", "Venus", "Earth", "Mars", "Jupiter", "Saturn", "Uranus", "Neptune")

# type vector
type <- c("Terrestrial planet", "Terrestrial planet", "Terrestrial planet", "Terrestrial planet", "Gas giant", "Gas giant", "Gas giant", "Gas giant")

# diameter vector
diameter <- c(0.382, 0.949, 1, 0.532, 11.209, 9.449, 4.007, 3.883)

# rotation vector
rotation <- c(58.64, -243.02, 1, 1.03, 0.41, 0.43, -0.72, 0.67)

# rings vector
rings <- c(FALSE, FALSE, FALSE, FALSE, TRUE, TRUE, TRUE, TRUE)

# construct a dataframe planet_df from all the above variables
planet_df <- data.frame(planets, type, diameter, rotation, rings)
```

`@sample_code`
```{r}
# select the values in the first row and second and third columns

# select the entire third column
```

`@solution`
```{r}
# select the values in the first row, and second and third columns
planet_df[1, c(2,3)]

# select the entire third column
planet_df$diameter
```

`@sct`
```{r}
ex() %>% check_output_expr("planet_df[1, c(2,3)]")
ex() %>% check_output_expr("planet_df$diameter")
success_msg("Good job, you'll become an expert with data frames")
```

---

## Lists

```yaml
type: NormalExercise
key: f67c593952
xp: 100
```

A list in R is similar to your to-do list at work or school: the different items on that list most likely differ in length, characteristic, type of activity that has to do be done.

A list in R allows you to gather a variety of objects under one name (that is, the name of the list) in an ordered way. These objects can be matrices, vectors, data frames, even other lists, etc. It is not even required that these objects are related to each other.

You can easily construct a list using the list() function. In this function you can wrap the different elements like so: `list(item1, item2, item3)`.

`@instructions`
* Put the objects my_vector, my_matrix and my_df into a list called my_list
* Make sure to print my_list

`@hint`
Look at the example in the last paragraph above the instructions. Just replace the names with the names of my_vector my_matrix and my_df

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# Vector with numerics from 1 up to 10
my_vector <- 1:10 

# Matrix with numerics from 1 up to 9
my_matrix <- matrix(1:9, ncol = 3)

# First 10 elements of the built-in data frame 'mtcars'
my_df <- mtcars[1:10,]

# Construct my_list with these different elements:


# print my_list to the console

```

`@solution`
```{r}
# solution code
# Vector with numerics from 1 up to 10
my_vector <- 1:10 
# Matrix with numerics from 1 up to 9
my_matrix <- matrix(1:9, ncol = 3)
# First 10 elements of the built-in data frame 'mtcars'
my_df <- mtcars[1:10,]

# Construct list with these different elements:
my_list <- list(my_vector, my_matrix, my_df)

# print my_list to the console
my_list
```

`@sct`
```{r}
ex() %>% check_output_expr("my_list")
ex() %>% check_expr("my_list") %>% check_result() %>% check_equal()
success_msg("You're starting great with lists!")
```

---

## Selecting elements from a list

```yaml
type: NormalExercise
key: 1891e8b53d
xp: 100
```

Your list will often be built out of numerous elements and components. Therefore, getting a single element, multiple elements, or a component out of it is not always straightforward. One way to select a component is using the numbered position of that component. For example, to "grab" the first component of my_list you type `my_list[[1]]`

Another way to check is to refer to the names of the components: `my_list[["my_vector"]]` selects the my_vector vector.

A last way to grab an element from a list is using the $ sign. The following code would select my_df from my_list: my_list$my_df.

Besides selecting components, you often need to select specific elements out of these components. For example, with `my_list[[1]][1]` you select from the first component of my_list the first element. This would select the number 1.

`@instructions`
* Grab the second element of my_list and print it to the console
* Grab the first column of the third component of my_list and print it to the console

`@hint`
Remember that you can select elements from list components using the following notation: `my_list[[3]][,2]`. This would grab the second column of my_df

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# Vector with numerics from 1 up to 10
my_vector <- 1:10 

# Matrix with numerics from 1 up to 9
my_matrix <- matrix(1:9, ncol = 3)

# First 10 elements of the built-in data frame 'mtcars'
my_df <- mtcars[1:10,]

# Construct list with these different elements:
my_list <- list(my_vector, my_matrix, my_df)

# Grab the second element of my_list and print it to the console


# Grab the first column of the third component of `my_list` and print it to the console
```

`@solution`
```{r}
# Vector with numerics from 1 up to 10
my_vector <- 1:10 

# Matrix with numerics from 1 up to 9
my_matrix <- matrix(1:9, ncol = 3)

# First 10 elements of the built-in data frame 'mtcars'
my_df <- mtcars[1:10,]

# Construct list with these different elements:
my_list <- list(my_vector, my_matrix, my_df)

# Grab the second element of my_list and print it to the console
my_list[[2]]

# Grab the first column of the third component of `my_list` and print it to the console
my_list[[3]][,1]
```

`@sct`
```{r}
ex() %>% check_output_expr("my_list[[2]]")
ex() %>% check_output_expr("my_list[[3]][,1]")
success_msg("You're great with lists!")
```
