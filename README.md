# Flap Standard Library

Core standard library functions for the Flap programming language.

## Functions

### contains(list, value)

Checks if a value exists in a list using tail recursion.

**Parameters:**
- `list` - The list to search in
- `value` - The value to find

**Returns:** `1` (yes) if found, `0` (no) if not found

**Example:**
```flap
contains([1, 2, 3], 2)  // -> 1 (yes)
contains([1, 2, 3], 4)  // -> 0 (no)
```

### filter(pred, list)

Keeps only elements where predicate returns yes.

**Parameters:**
- `pred` - A predicate function
- `list` - The list to filter

**Example:**
```flap
filter(x => x > 2, [1, 2, 3, 4])  // -> [3, 4]
```

### map(f, list)

Applies a function to each element of a list.

**Parameters:**
- `f` - The function to apply
- `list` - The list to map over

**Example:**
```flap
map(x => x * 2, [1, 2, 3])  // -> [2, 4, 6]
```

### reduce(f, list, init)

Folds a list with a binary function and initial value using tail recursion.

**Parameters:**
- `f` - Binary function taking accumulator and current element
- `list` - The list to reduce
- `init` - Initial accumulator value

**Example:**
```flap
reduce(acc, x => acc + x, [1, 2, 3, 4], 0)  // -> 10
```

### reverse(list)

Reverses a list using slice notation.

**Parameters:**
- `list` - The list to reverse

**Example:**
```flap
reverse([1, 2, 3])  // -> [3, 2, 1]
```

## General

* License: BSD-3
