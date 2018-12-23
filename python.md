# Modules
- Just a .py file e.g. `mod.py`
- import by `import mod.py`
- by default, objects must by accessed via `mod.object`, but `from mod import object[,object...]` can be used to import them properly.
- `*` can be used in python 2, but isn't recommended
- can also import as, with expected syntax, for both objects and whole modules
- `_` keeps objects local

# Packages
- A folder containing modules
- Modules can be refered to via dot notation and used normally
- Or they can by imported via `from package import module[,module...]`
- If there is a file called `__init__.py` in a package, it will be run on import
- `*` finds a list called `__all__` in the `__init.py__` file, and imorts all objects listed in it. Not recommended.
- Packages can be nested.

# Utility
- `dir()` lists all symbols in local symbol table
- `repr()` tries to print the string that would make the object
- `str()` prints as a strong

# Base types
- bool (`True`, `False`)
- int
- float
- complex
- sequences ([list], (tuple), "str", etc:
  - operations:
    - `x in s`
    - `s + t`
    - `s[0]`
    - `s[0,3]`
    - `len(s)`
    - `s[i] = x`
    - `s.append(x)`
    - `del s[1:3]`
    - `s.insert(i,x)`
    - `s.remove(x)`
- {dict}:
  - operations:
    - `len(d)`
    - `d[key]`
    - `d[key] = value`
    - `del d[key]`
    - `key in d`
    - `d.items`, `d.keys`, `d.values`
    - `iter(d)`
    - `d.update(e)`
- set
- various byte sequences
- `None`

# Operators
- boolean: `and`, `or`, `not`
- bitwise: `|`, `&`
- `in`, `not in`
- `+` for concatenation

# Control flow
- if, while, for, try, with
- functions can have default params
- functions created by `def function(): `
- functions are first class objects

# OOP
- classes:
  - defined via `class Foo(parent):`
  - classes are executed on creation
- methods:
  - methods are defined in classes
  - if you call a method through an instance (`m.func`, it adds `self` to the argument list
  - `self.name = value` can be used to set instance attributes
