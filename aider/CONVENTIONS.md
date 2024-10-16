Python conventions:
* Avoid many nested loops, use itertools.product and similar instead.
* Avoid many nested if-elif-else statements, use dictionaries instead.
* Avoid many nested built-in types, use namedtuples, classes, and dataclasses instead.
* Never use map and filter, use list comprehensions instead.
* Never use lambda, use def instead.
* Prefer list comprehensions over for loops.
* Prefer f-strings over str.format.
* Prefer classmethods to write constructors for classes.
* Finish all functions and classes with return statements.
* Write google-style docstrings for all files, functions, class attributes, public and dunder methods.
    - Class docstrings should include a description of the class, its attributes, public and dunder methods.
    - Multi-line docstring summary line should start at the first line.
    - Summary line of functions and methods should be in imperative mood.
    - When returning several values as a tuple, write each output in a separate line in the docstring. Example:

    ```python
    ... -> tuple[int, str]:
        """
        ...
        Returns:
            int: ...
            str: ...
        """
        ...
    ```

* Use type hints for all function arguments and return values.
    - Do not type hint a None return value of a function.
    - Do not import List and Tuple from typing, use the built-in list and tuple.
    - Do not import Union from typing, use the built-in |.

Typst Conventions:
* Do NOT suggest to recompile the .typ file: "typst compile ...". DON'T. All files are being watched and are automatically recompiled after changes.

