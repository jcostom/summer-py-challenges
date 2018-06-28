# Ready to Welcome our New Robotic Overlords?

Yeah, me neither.

So, so what's going on here?

Since our first condition says the number has to be divisible y *both* 3 and 5, that's the same as saying the number is divisible by 15. Cool - now we can do a single test instead of 2.

Next, we test for divisibility by 3 and 5, and lastly if all else fails, we return the number as a string, using the `str()` function.

```python
def fizzbuzz(number):
    if number % 15 == 0:
        return "Fizz Buzz"
    elif number % 3 == 0:
        return "Fizz"
    elif number % 5 == 0:
        return "Buzz"
    else:
        return str(number)


# These "asserts" using only for self-checking and not necessary for auto-testing
if __name__ == '__main__':
    assert checkio(15) == "Fizz Buzz", "15 is divisible by 3 and 5"
    assert checkio(6) == "Fizz", "6 is divisible by 3"
    assert checkio(5) == "Buzz", "5 is divisible by 5"
    assert checkio(7) == "7", "7 is not divisible by 3 or 5"
    print("No Errors? You did it!")
``` 