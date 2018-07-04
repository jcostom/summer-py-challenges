# My solution

Maybe yours is different, but this one is mine.

```python
def oddoreven(num):
    if num % 2 == 0:
        return 'even'
    else:
        return 'odd'


number = int(input("Input a number: "))
print("You input {}. That's an {} number.".format(number, oddoreven(number)))
```