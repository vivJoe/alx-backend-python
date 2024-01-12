Variable (Type) Annotations
This project contains tasks for learning to use variable/type annotations in Python 3.

Tasks To Complete
 0. Basic annotations - add
0-add.py contains a type-annotated function add that takes a float a and a float b as arguments and returns their sum as a float..

 1. Basic annotations - concat
1-concat.py contains a type-annotated function concat that takes a string str1 and a string str2 as arguments and returns a concatenated string.

 2. Basic annotations - floor
2-floor.py contains a type-annotated function floor which takes a float n as argument and returns the floor of the float.

 3. Basic annotations - to string
3-to_str.py contains a type-annotated function to_str that takes a float n as argument and returns the string representation of the float.

 4. Define variables
4-define_variables.py contains a script that define and annotate the following variables with the specified values:

a, an integer with a value of 1.
pi, a float with a value of 3.14.
i_understand_annotations, a boolean with a value of True.
school, a string with a value of “Holberton”.
 5. Complex types - list of floats
5-sum_list.py contains a type-annotated function sum_list which takes a list input_list of floats as argument and returns their sum as a float.

 6. Complex types - mixed list
6-sum_mixed_list.py contains a type-annotated function sum_mixed_list which takes a list mxd_lst of integers and floats and returns their sum as a float.

 7. Complex types - string and int/float to tuple
7-to_kv.py contains a type-annotated function to_kv that takes a string k and an int OR float v as arguments and returns a tuple. The first element of the tuple is the string k. The second element is the square of the int/float v and should be annotated as a float.

 8. Complex types - functions
8-make_multiplier.py contains a type-annotated function make_multiplier that takes a float multiplier as argument and returns a function that multiplies a float by multiplier.

 9. Let's duck type an iterable object
9-element_length.py contains an annotation of the function's (shown below) parameters and return values with the appropriate types.

def element_length(lst):
  return [(i, len(i)) for i in lst]
 10. Duck typing - first element of a sequence
100-safe_first_element.py contains an augmentation of the following code with the correct duck-typed annotations:

# The types of the elements of the input are not know
def safe_first_element(lst):
    if lst:
        return lst[0]
    else:
        return None
 11. More involved type annotations
101-safely_get_value.py contains a script that includes the code below with type annotations added to it.

def safely_get_value(dct, key, default = None):
  if key in dct:
      return dct[key]
  else:
      return default
 12. Type Checking
102-type_checking.py contains the code below and uses mypy to validate it and apply any necessary changes.

def zoom_array(lst: Tuple, factor: int = 2) -> Tuple:
  zoomed_in: Tuple = [
      item for item in lst
      for i in range(factor)
  ]
  return zoomed_in


array = [12, 72, 91]

zoom_2x = zoom_array(array)

zoom_3x = zoom_array(array, 3.0)

