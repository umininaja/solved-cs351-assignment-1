Download Link: https://assignmentchef.com/product/solved-cs351-assignment-1
<br>
5/5 - (1 vote)

<table>

 <tbody>

  <tr>

   <td></td>

  </tr>

  <tr>

   <td></td>

  </tr>

  <tr>

   <td></td>

  </tr>

 </tbody>

</table>




<pre># Python Warmup Assignment</pre>

Solve the following problems in Python 3.6+ .

In addition to making sure that your code gives the correct solution, each solution must meet the following conditions.

1. Your function parameters must be [type- hinted](https://docs.python.org/3.6/library/typing.html]). These need not be perfect, but should be generally correctly describe your input and output.2. Your functions must have a doc-string describing what the function does. Keep is succinct and concise.3. Use a auto-formatter such as [black](https://pypi.org/project/black/) or [autopep8](https://pypi.org/project/autopep8/).4. Write atleast 2 simple [doctests](https://docs.python.org/3.6/library/doctest.html) per solution to verify that your code is working correctly.5. Use descriptive variable names.

Here is an example of what your code should look like.

<pre>For example```pythonfrom typing import List</pre>

def average(num_list: List[int]) -&gt; float: “””Finds the average of a list of numbers.

<pre>    doctests:    &gt;&gt;&gt; average([1,2,3,4,5])    3.0    &gt;&gt;&gt; average([0])    0.0    """</pre>

<pre>    list_sum = sum(num_list)    list_size = len(num_list)    avg = list_sum/list_size    return avg</pre>

<pre>if __name__ == "__main__":    import doctest</pre>

<pre>    doctest.testmod()```</pre>

## Problem 1Write a function to break down a string into a list of characters.

<table>

 <tbody>

  <tr>

   <td></td>

  </tr>

  <tr>

   <td></td>

  </tr>

  <tr>

   <td></td>

  </tr>

 </tbody>

</table>

<pre>```Input: "abc"Output: ['a','b','c']```</pre>

## Problem 2Write a function to reverse output of the problem 1 back into a string “`Input: [‘a’,’b’,’c’]Output: “abc”“`

## Problem 3Write a function generate a list of n random numbers. Use the inbuilt `random` module.

<pre>```Input: 5Output: [5,2,3,1,5]```</pre>

## Problem 4Write a function a sort a given list of numbers in descending order.

<pre>```Input:  [1,2,3,4,5]Output: [5,4,3,2,1]```</pre>

## Problem 5Write a function to get frequency of each numbers in a list of numbers. Use a python `dict` to solve this.

<pre>```Input:  [1,1,3,2,3,2,3,2,2]Output: {1: 2, 3: 3, 2: 4}```</pre>

## Problem 6Write a function to get all the unique elements from given list. Your solution must use `set` to solve this.

<pre>```Input:  [1,1,3,2,3,2,3,2,2]Output: {1,2,3}</pre>

“`

## Problem 7Write a function to get the first repeating element from list. Your solution must use `set` to solve this.

<pre>```Input:  [1,2,3,4,5,1,2]Output: 1```</pre>

## Problem 8

<table>

 <tbody>

  <tr>

   <td></td>

  </tr>

  <tr>

   <td></td>

  </tr>

  <tr>

   <td></td>

  </tr>

 </tbody>

</table>

Write a function that takes an integer n and output a `dict` containing keys from 0,2 … to n and each key is mapped to a list containing the square and cube of the number.

<pre>```Input: 3Output:{</pre>

<pre>    0:[0,0],    1:[1,1],    2:[4,8],    3:[9,27]</pre>

} “`

## Problem 9Given two lists of equal size, write a function to create tuples of each consecutive element having same index. Use `zip` in some capacity to solve this.

“`Input: [1,2,3,4], [‘a’,’b’,’c’,’d’]Output: [(1,’a’), (2,’b’), (3,’c’), (4,’d’)] “`

## Problem 10Write a function that uses list comprehension to generate the squares of 0 to n.

<pre>```Input : 5Output : [0, 1, 4, 9, 16, 25]```</pre>

## Problem 11Write a function that uses dictionary comprehension to generate a mapping from (0 to n) to their squares.

“`Input : 5Output : {0:0, 1:1, 2:4, 3:9, 4:16, 5:25} “`

<pre>## Problem 12.Write a `class` such that :</pre>

1. The initializer takes an arbitrary list of atomic values as input and saves it in a instance variable.2. Has a method called `apply` which has the following functionality:

1. Accepts a function as a parameter. You can use a lambda function.

2. Applies the function to saved list and return the output. The instance variable must not be modified.

3. If it fails `raise` an `Exception` with a custom error message. You can use `try` and `except` here.

<pre>```pythondef sq(x):</pre>

return x**2

<table>

 <tbody>

  <tr>

   <td></td>

  </tr>

  <tr>

   <td></td>

  </tr>

 </tbody>

</table>

<pre>c1 = MyClass([1,2,3,4])</pre>

print(c1.apply(lambda x:x**2)) [1,4,9,16]

c2 = MyClass([‘a’,’b’,’c’])c2.apply(sq) ———————————————————————– —-TypeErrorlast)….….Exception: Custom Error

<pre>Traceback (most recent call</pre>

“`

## Problem 13Write a function takes as input a list of words and upper-cases each word. Use `functools.map` in some capacity to solve this.

<pre>```Input : ['aa','bb','cd','e']Output : ['AA', 'BB', 'CD', 'E']```</pre>

## Problem 14:Write a function to find the product of all the numbers in a list using `functools.reduce` in some capacity.