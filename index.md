## Welcome to Lavla!
[![Documentation Status](https://readthedocs.org/projects/lavla/badge/?version=latest)](http://lavla.readthedocs.io/en/latest/?badge=latest)
Lavla is a simple web framework for Python.  You can create templates and more with this framework.

#### Starting off with Lavla
To start you will want a source.  You can either use a file or a string.
```python
from lavla import *
page = lavla('My Website','page1','Page 1')
page.new('page1',['C:','mywebsite'],['Website Name','{nm}'])
```

Now if there is not a folder in the C:/ directory this will create a folder at this file path: ```C:/mywebsite```.  The variables in this function are:
```python
String 'name',
Array 'path',
Array 'pre'
```
Pre is for asigning variables to your script.  If the ```'page1.html.lavla'``` file had this code:
```html
<p>{0} : {1}</p>
```
It will output this:
```
Website Name : My Website
```
