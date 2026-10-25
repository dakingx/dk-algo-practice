The code template is as follows:

```python
def {$function_name}({$parameters}):
    """This function contains the core logic of the algorithm.
    """
    pass

def main():
    """
    1. Parse standard input to parameters
    2. Invoke the algorithm function with the parameters
    3. Print the result to standard output
    """
    pass

if __name__ == "__main__":
    main()
```

The following points should be noted:

- `{$function_name}(...)` — contains the core algorithm. The parameter names should match the problem's input parameters.

- `main()` — reads from stdin, calls the algorithm function, prints result to stdout.

- Replace `{$function_name}` with a semantic name describing the algorithm logic (e.g., `count_inversions`, `find_max_subarray`).
