### Generate PowerSet from a set
 
```
# using recursion

elements = list(map(int, input().split()))


def get_power_set(elements: list) -> list:
    if not elements:
        return [[]]
    excluding_elem = get_power_set(elements[1:])
    including_elem = [[elements[0]] + subset for subset in get_power_set(elements[1:])]
    return excluding_elem + including_elem


print(get_power_set(elements))
```

```
# using itertools - PENDING!

```
### Generate all permutations of a set
```

```

