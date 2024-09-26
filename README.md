# TinyTest
A small testing framework for Dyalog APL. [Why?](CONTEXT.md)

## Usage
Create a namespace of functions, whose names begin `Test_`, that return `1` if they pass and `0` if they fail.

```
 Test_Equal←{
    3=3   ⍝ Not a great example, but you get the idea
 }
```

Call the Run function with a right argument reference to that namespace containing your test functions.

```
Run #.tests
```

The optional left argument controls debug behaviour:
- 0 (default): Ignore errors, simply report results
- 1: Stop on errors and failures
- 2: Stop before each test

## Installation

### Tatin
TinyTest is provided as a Tatin package (not yet).

### Get
You can also bring TinyTest into your active workspace with the `]Get` user command (also not tested).
