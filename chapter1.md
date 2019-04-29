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
