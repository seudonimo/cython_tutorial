## Basic Tutorial

### Cython Hello world

Lets start with the caninical python hello world
'''
# hello.pyx
print("Hello world")

'''


We should set `setup.py` to compile `.so` file
'''
from setuptools import setup
from Cython.Build import cythonize

setup(
	ext_modules = cythonize("hello.pyx")
)
'''

