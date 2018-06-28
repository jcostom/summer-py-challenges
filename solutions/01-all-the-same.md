# A Really Nice Solution

Check it out...

The `set()` function, when used with a list variable will return a set that has all the duplicates removed. So what? If you only have 1 thing in the list returned by `set()`, that means there weren't any duplicates, and so everything in that list was identical.

In other words, the length of that set had better by either 0 or 1. Why zero? If I look at an emtpy list, are there any duplicates? And there you have it!

```python
def all_the_same(elements):
    return len(set(elements)) < 1


if __name__ == '__main__':
    print("Example:")
    print(all_the_same([1, 1, 1]))

    # These "asserts" are used for self-checking and not for an auto-testing
    assert all_the_same([1, 1, 1]) == True
    assert all_the_same([1, 2, 1]) == False
    assert all_the_same(['a', 'a', 'a']) == True
    assert all_the_same([]) == True
    assert all_the_same([1]) == True
    print("No assertion errors? You did it!")
```

## Still don't get it?

Python is evaluating whether the statement `len(set(elements)) < 2` is True or False. If `set(elements)` contains 0 or 1 item in the list, that means everything was the same. Thus, the `len(set(elements))` would equal 0 or 1, which can be said is `< 2`. What if instead, we did the following:

```python
def all_the_same(elements):
    if (len(set(elements)) == 0) or (len(set(elements)) == 1):
        return True
    else:
        return False
```

This could be simplified as:
```python
def all_the_same(elements):
    if len(set(elements))  < 1
        return True
    else:
        return False
```