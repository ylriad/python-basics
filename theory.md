# Python basics

### The 1<sup>st</sup> lesson. Introduction.

- Python code is interpreted at runtime. Each line is only checked (executed) when it runs.
- The fully-qualified name of a function includes the module or file it’s in. 
    - Example: the function `foo()` in `binky.py` is called as `binky.foo()`.
    - Example: `sys.exit()` calls the `exit()` function from Python’s built-in sys module, which stops the script early.
    - You can also import specific functions directly: `from sys import argv, exit`.


**`sys` module**  
- a very standard module  
- `sys.argv` contains command line arguments. `sys.argv[0]` - the name of the script, `sys.argv[1]` - the first argument.   
- `len(sys.argv)` - shows the number of arguments.  


**Functions**
- `def` is for defining a function. 

Example:

```
def repeat(s, exclaim):
    """
    Returns the string 's' repeated 3 times.
    If exclaim is true, add exclamation marks.
    """

    result = s + s + s      # can also use "s * 3" which is faster 
    if exclaim:
        result = result + '!!!'
    return result
```

<ins>Explanation. </ins>

'repeat' - is the name of the function. `s` and `exclaim` are arguments.  
"""....""" - the docstring, describing what the function does.


A code that calls the previous function:

```
def main():
    print(repeat('Yay', False))      ## YayYayYay
    print(repeat('Woo Hoo', True))   ## Woo HooWoo HooWoo Hoo!!!

main()
```

**Python help**

- There are many modules and packages which are bundled with a standard installation of the Python interpreter. [Standard Library modules](https://docs.python.org/3/library/)
- Functions `help()` and `dir()`show important info about arguments, functions and modules. 





### The 2<sup>nd</sup> lesson. Strings.

*(Coming soon — working on strings next!)*




