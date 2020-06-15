# Coding Style

The Data Science Team works to maintain
a consistent code style for code readability
and maintenance.

## PEP 8 Code Style

For all coding, we follow PEP 8 style guidelines, outlined in the following resources.

* [PEP 8 -- Style Guide for Python Code](https://www.python.org/dev/peps/pep-0008/)

* [How to Write Beautiful Python Code With PEP 8](https://realpython.com/python-pep8/)

## NumPy Docstring Formatting

We also use the NumPy style formatting for docstrings, as outlined 
[here](https://www.sphinx-doc.org/en/master/usage/extensions/example_numpy.html).

## Additional Code Style Conventions

* Keep line lengths at 120 characters.

* Access Pandas dataframes with strings and brackets.

* Single word or snake_case is best for variable names.

* Use “_df” suffix for pandas dataframe variables names.

* Use “_ts” suffix for time series variables names.

* When a variable or function has a long list of arguments, 
keep them indented in a single-item vertical list separated by commas. 
Offset the list from the function names using one or two indents (4/8 spaces). 
This makes it easier to spot the arguments.

* **Single-quotes vs. double-quotes:** While either can be used, we prefer to use double quotes 
as there may be cases where you need to embed quotes within 
quotes and in those rare cases, we find that the single 
quote within the double quote is easier to read “ ‘ “ than the opposite case ‘ “ ‘.

## Automating Code Formatting 

Given that formatting code can be a time sink, we try to automate
as much of the styling as possible.

PyCharm has some tools for automating code styling, 
which will be further explored by the Data Science Team.

## Python Version

The minimum python version that we will support is 3.6.



