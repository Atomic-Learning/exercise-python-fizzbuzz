Write an if/elif/else block that prints different outputs based on divisibility:


* If a number is divisible by both 3 and 5, print `FizzBuzz`{.python}
* If it is divisible by 3 only, print `Fizz`{.python}
* If it is divisible by 5 only, print `Buzz`{.python}
* Otherwise, print the number itself

Test your code with different values of `a`{.python}. For example:

* `a = 3` should print `Fizz`{.python}
* `a = 10` should print `Buzz`{.python}
* `a = 15` should print `FizzBuzz`{.python}
* `a = 7` should print `7`{.python}

## Hints

> [!HIDDEN]
> * Think carefully about the order of your conditions.
> * Use the modulo operator `\%`{.python} to check if a number is divisible by another (if `n % d == 0`{.python}, then `n`{.python} is divisible by `d`{.python})

# Your Code

```py-cell
a = 1

# Write your if/elif/else block here
```

# Sample Solution

> [!HIDDEN]
>
> ## Why Order Matters
>
> The key to this problem is understanding that once a condition is `True`{.python}, the remaining conditions are not checked. Because of this, we must check for divisibility by both 3 and 5 first, before checking for just 3 or just 5. Otherwise, a number like 15 would match the "divisible by 3" condition and never reach the "divisible by both" check. This demonstrates a general principle in if/elif/else blocks: more specific conditions should be checked before more general ones.
> 
> ## The Solution
> 
> Here is one correct solution:
> 
> ```py-cell
> a = 15
> 
> if a % 3 == 0 and a % 5 == 0:
>     print("FizzBuzz")
> elif a % 3 == 0:
>     print("Fizz")
> elif a % 5 == 0:
>     print("Buzz")
> else:
>     print(a)
> ```

> Change the value of the variable `a` to test different cases (suggested values: 15, 3, 10, 7).
