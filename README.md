# NBDEV TEST!
> This showcases how great nbdev works!


This file will become your README and also the index of your documentation.

## Install

`pip install your_project_name`

## How to use

Car can be instantitated like this:

```python
car = Car()
car.get_location()
```




    'at home'



And then we drive it to a new, secret location:

```python
get_car_to_important_location(car,IMPORTANT_STRING)
```

    drove to Munich





    'car is now at Munich'



# How to test


Testing is pretty simple and straight forward with this:



```python
from nbdev_template.test import test_location
```

```python
test_location(get_car_to_important_location(car,IMPORTANT_STRING)) 
```

    drove to Munich


```python
test_location(car.num_wheels)
```


    ---------------------------------------------------------------------------

    AssertionError                            Traceback (most recent call last)

    <ipython-input-8-489a4616d12c> in <module>
    ----> 1 test_location(car.num_wheels)
    

    ~/Documents/GitHub Personal/nbdev_documentation_example/nbdev_template/test.py in test_location(location)
          5 # Cell
          6 def test_location(location):
    ----> 7     assert type(location) == str, 'looks like the locations isnt a string'
    

    AssertionError: looks like the locations isnt a string

