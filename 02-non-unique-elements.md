# Non-Unique Elements

For your next task, you're given a list. Maybe all of the elements are unique, maybe there are duplicates. Your job? Figure out which elements have duplicates in the list and report back.

Examples:

[1, 2, 1, 1, 3, 4] -> [1]
[1, 1, 2, 2, 3, 4, 3] -> [1, 2, 3]
[1, 2, 3, 4, 5, 6, 7] -> []

Here's your template, with built-in checks:

```python
def nonunique(data):
    # Your Code Here
    return some_list

# Some hints
# You can use list.count(element) method for counting.
# Create new list with non-unique elements
# Loop over original list


if __name__ == "__main__":
    # These "asserts" using only for self-checking and not necessary for auto-testing
    assert list(nonunique([1, 2, 3, 1, 3])) == [1, 3, 1, 3], "1st example"
    assert list(nonunique([1, 2, 3, 4, 5])) == [], "2nd example"
    assert list(nonunique([5, 5, 5, 5, 5])) == [5, 5, 5, 5, 5], "3rd example"
    assert list(nonunique([10, 9, 10, 10, 9, 8])) == [10, 9, 10, 10, 9], "4th example"
    print("It is all good. Let's check it now")
```