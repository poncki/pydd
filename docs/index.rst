.. pydd documentation master file, created by
   sphinx-quickstart on Wed Aug 17 23:07:17 2016.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to pydd's documentation!
================================

Contents:

.. toctree::
   :maxdepth: 2


Disassembly of func:
  9           0 LOAD_FAST                0 (arg1)
              3 STORE_FAST               1 (arg2)

 11           6 LOAD_GLOBAL              0 (print)
              9 LOAD_FAST                1 (arg2)
             12 CALL_FUNCTION            1 (1 positional, 0 keyword pair)
             15 POP_TOP

 12          16 LOAD_GLOBAL              0 (print)
             19 LOAD_GLOBAL              1 (type)
             22 LOAD_FAST                0 (arg1)
             25 CALL_FUNCTION            1 (1 positional, 0 keyword pair)
             28 CALL_FUNCTION            1 (1 positional, 0 keyword pair)
             31 POP_TOP
             32 LOAD_CONST               0 (None)
             35 RETURN_VALUE


   Disassembly of func:
  9           0 LOAD_FAST                0 (arg1)
              3 STORE_FAST               1 (arg2)

 11           6 LOAD_GLOBAL              0 (print)
              9 LOAD_FAST                1 (arg2)
             12 CALL_FUNCTION            1 (1 positional, 0 keyword pair)
             15 POP_TOP

 12          16 LOAD_GLOBAL              0 (print)
             19 LOAD_GLOBAL              1 (type)
             22 LOAD_FAST                0 (arg1)
             25 CALL_FUNCTION            1 (1 positional, 0 keyword pair)
             28 CALL_FUNCTION            1 (1 positional, 0 keyword pair)
             31 POP_TOP
             32 LOAD_CONST               0 (None)
             35 RETURN_VALUE

>>> dis(t1.f1)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
AttributeError: module 't1' has no attribute 'f1'
>>> dis(t1.func)
  9           0 LOAD_FAST                0 (arg1)
              3 STORE_FAST               1 (arg2)

 11           6 LOAD_GLOBAL              0 (print)
              9 LOAD_FAST                1 (arg2)
             12 CALL_FUNCTION            1 (1 positional, 0 keyword pair)
             15 POP_TOP

 12          16 LOAD_GLOBAL              0 (print)
             19 LOAD_GLOBAL              1 (type)
             22 LOAD_FAST                0 (arg1)
             25 CALL_FUNCTION            1 (1 positional, 0 keyword pair)
             28 CALL_FUNCTION            1 (1 positional, 0 keyword pair)
             31 POP_TOP
             32 LOAD_CONST               0 (None)
             35 RETURN_VALUE





>>> dis(t1)
Disassembly of func:
  9           0 LOAD_FAST                0 (arg1)
              3 STORE_FAST               1 (arg2)

 12           6 LOAD_GLOBAL              0 (print)
              9 LOAD_GLOBAL              1 (type)
             12 LOAD_FAST                0 (arg1)
             15 CALL_FUNCTION            1 (1 positional, 0 keyword pair)
             18 CALL_FUNCTION            1 (1 positional, 0 keyword pair)
             21 POP_TOP
             22 LOAD_CONST               0 (None)
             25 RETURN_VALUE

>>> dir(t1)
['__builtins__', '__cached__', '__doc__', '__file__', '__loader__', '__name__', '__package__', '__spec__', 'a', 'func']
>>> dis(t1.func)
  9           0 LOAD_FAST                0 (arg1)
              3 STORE_FAST               1 (arg2)

 12           6 LOAD_GLOBAL              0 (print)
              9 LOAD_GLOBAL              1 (type)
             12 LOAD_FAST                0 (arg1)
             15 CALL_FUNCTION            1 (1 positional, 0 keyword pair)
             18 CALL_FUNCTION            1 (1 positional, 0 keyword pair)
             21 POP_TOP
             22 LOAD_CONST               0 (None)
             25 RETURN_VALUE



Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`

