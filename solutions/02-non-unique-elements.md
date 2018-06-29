So, how does this solution work?

1. First, we create a list to hold our set of items that have duplicates in the original list.
2. Next, we run through that list, 1 item at a time. Using the `count()` function, we find out if there's more than 1 of that item in the list If there is, we add the item to the list of duplicates.
3. We return the list of duplicates.

```python
def nonunique(data):
    duplist = []
    for i in data:
        if data.count(i) > 1:
            duplist.append(i)
    return duplist


if __name__ == "__main__":
    # These "asserts" using only for self-checking and not necessary for auto-testing
    assert list(nonunique([1, 2, 3, 1, 3])) == [1, 3, 1, 3], "1st example"
    assert list(nonunique([1, 2, 3, 4, 5])) == [], "2nd example"
    assert list(nonunique([5, 5, 5, 5, 5])) == [5, 5, 5, 5, 5], "3rd example"
    assert list(nonunique([10, 9, 10, 10, 9, 8])) == [10, 9, 10, 10, 9], "4th example"
    print("It is all good. Let's check it now")
```
