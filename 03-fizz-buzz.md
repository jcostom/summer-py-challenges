# Fizz Buzz

Today, we're teaching robots about division. The robots like word games, so here's the one they play with division. You're going to write a function to return words or a number based on the following rules:

1. If the number is divisible by 3 and 5 return, "Fizz Buzz".
2. If the number is divisible by 3 return, "Fizz".
3. If the number is divisible by 5 return, "Buzz".
4. If the number (as a string) if it is not divisible by either 3 or 5.

Some examples:

* fizzbuzz(15) -> "Fizz Buzz"
* fizzbuzz(21) -> "Fizz"
* fizzbuzz(100) -> "Buzz"
* fizzbuzz(97) -> "97"

Hint: To return a number as a string, use str().

Another Hint: Don't forget about modulo arithmetic. Remember when you first did division? Like say you did 7 / 4. You'd have said 1, remainder 3. That's what mod arithmetic cares about - remainders. So, 7 % 4 = 3 (since 7/4 = 1r*3*). What do you think the result of 9 % 3 would be?

Here's a template to work from:

```python
def fizzbuzz(number):
    # Your code goes here


# These "asserts" using only for self-checking and not necessary for auto-testing
if __name__ == '__main__':
    assert checkio(15) == "Fizz Buzz", "15 is divisible by 3 and 5"
    assert checkio(6) == "Fizz", "6 is divisible by 3"
    assert checkio(5) == "Buzz", "5 is divisible by 5"
    assert checkio(7) == "7", "7 is not divisible by 3 or 5"
    print("No Errors? You did it!")
``` 