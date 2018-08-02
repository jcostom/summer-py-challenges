# All the Same

## Your challenge awaits...

Your challenge is relatively simple. You need to determine if all of the items fed to you in a `list` variable are the same. Here's a template you can follow, including some code to check your work.

```python
def all_the_same(elements):
    # your code here


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

## Hint...

If all the items in a list were the same, how many items would the list that gets returned by the set(list) function be? If it's more than 1, you're doing something wrong.