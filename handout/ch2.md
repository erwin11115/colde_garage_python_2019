CH2
===
> handout source https://hackmd.io/@michael1017/ryF_RAdwH
###### tags: `colde_garage_python_2019`
# String
## What is String
```python=
a = "apple"
print( type(a) )
```
## Operation for String
```python=
a = "apple"
b = "banana"
# add
print(a + b)
# multiply
print(a * 2 + b)
# in
print("pp" in a)
```
```
applebanana
appleapplebanana
True
```
## Slice
### Get element from string
```python=
variable = "my_string"
print(variable[3])
```
```
s
```
### How to use slice
![](https://i.imgur.com/ftlbOlW.png)

```python=
variable[start:end:step]
```
```python=
variable = "0123456789"
print(variable[2:])
print(variable[-2:])
print(variable[:2])
print(variable[:-2])
print(variable[2:5])
print(variable[::3])
```
```
23456789
89
01
01234567
234
0369
```
### How about print from 9 to 0 ???
```python=
variable = "0123456789"
print(variable[::-1])
```
### Not only string has slice
* List
* Tuple
* Dictionary
## Useful Function for string
### len()
```python=
s = "abc"
print(len(s))
```
```
3
```
### split()
* default 空白字元
```python=
s = "a b c"
print(s.split())
```
```
['a', 'b', 'c']
```
* 自訂引數 split('?')
```python=
s = "a,b,c"
print(s.split(','))
```
```
['a', 'b', 'c']
```
### join()
* '??'.split(list)
```python=
list = ["apple", "banana", "candy"]
print('^ '.join(list))
```
```
apple^ banana^ candy
```
### replace()
your_string.replace(old, new[, count])
```python=
your_string = "helLo woRldooooo"
old = "o"
new = "kkkk"
result1 = your_string.replace(old, new)
result2 = your_string.replace(old, new, 3)
print(result1 + "\n" + result2)
```
```
helLkkkk wkkkkRldkkkkkkkkkkkkkkkkkkkk
helLkkkk wkkkkRldkkkkoooo
```
## uppercase and lowercase characters
* your_string.title() 所有單詞第一字大寫
* your_string.upper()
* your_string.lower()
* your_string.swapcase() 大小寫對調
* your_string.center(len) 
* your_string.ljust(len)
* your_string.rjust(len)
```python=
your_string = "helLo woRld"
len = 30
print(your_string.title())
print(your_string.upper())
print(your_string.lower())
print(your_string.swapcase())
print(your_string.center(len)) 
print(your_string.ljust(len))
print(your_string.rjust(len))
```
```
Hello World
HELLO WORLD
hello world
HELlO WOrLD
         helLo woRld
helLo woRld
                   helLo woRld
```
### Still a lot of thing
https://www.w3schools.com/python/python_strings.asp
# Data structure
## List
```python=
my_list = ["aaa", "bbb", "ccc"]
empty_list = []
print(my_list[1:])
```

## Tuple
```python=
my_tuple = ("aaa", "bbb", "ccc")
empty_tuple = ()
print(my_tuple[1:])
```

## Dictionary
```python=
my_dictionary = {"a":"apple", "b":"banana"}
empty_dictionary = {}
print(my_dictionary[1:])
```
## Tutorial from w3schools
https://www.w3schools.com/python/python_lists.asp
https://www.w3schools.com/python/python_tuples.asp
https://www.w3schools.com/python/python_dictionaries.asp
## map
https://www.w3schools.com/python/ref_func_map.asp  
input  
```
1 2 3 4
```
code  
```python=
s = input();
my_list = list(map(int, s.split()))
print(my_list)
```
output
```
[1, 2, 3, 4]
```