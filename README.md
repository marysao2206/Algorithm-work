## Exercise 1
- Reverse this string 
```python
text = "Hello Baby"
reverseText = ""
lastIndex = len(text) - 1

for index in range(len(text)): 
    reverseText += text[lastIndex - index]
print(reverseText)

# Output: ybab olleh
```
- Reverse this string using negative index 
``` python
text = "Hello Baby"
reverseText = ""
for index in range(1,len(text) + 1): 
    reverseText += text[-index]
print(reverseText)

# Output: ybab olleh 
```

## Exercise 2
- How many average of number in list?
```python
arr = [5, 7, 8, 4, 3]
average = 0
sum = 0
for value in arr:
    sum += value
average = sum / len(arr)
print(average)

# Output: 5.4
```
<!-- ## arr = [5,7,8,4,3] -->
- Sum all number in array?
```python
arr = [5, 7, 8, 4, 3]
sum = 0
for value in arr:
    sum += value
print(sum)

# Output : 27
```
## Exercise 3
- finds and prints all even numbers in the list
```python
arr = [5, 7, 8, 4, 3]
for value in arr:
    if value % 2 == 0:
        print(value)

# Output: 8 , 4 
```


## Exercise: 4
- How many average of number in list?
    - Output: 5.4
```python
arr = [5,7,8,4,3]
average = 0
sum = 0
for value in arr:
    sum += value
average = sum / len(arr)
print(average)
```
## Exercise:5
- arr = [{'name': 'bopha', 'age': 18}, {'name': 'thida', 'age': 12},{'name': 'kanha', 'age': 16}]

- What is the data type of each item inside the list `arr`?
    - Output :
bopha
thida
kanha

```python
for dics in arr:
    print(dics['name'])
```
## Exercise: 6
- Sum all number
    - Output : 27
```python
arr = [5,7,8,4,3]
sum = 0
for value in arr:
    sum += value
print(sum)
```


## Exercise: 7

- finds and prints all even numbers in the list
  - Expected Output: 8 , 4 
```python
arr = [5, 7, 8, 4, 3]
for value in arr:
    if value % 2 == 0:
        print(value)
```
## Exercise: 8

- find minimum number in the list
  - Expected Output: 3
```python
arr = [10, 40, 20, 4,3]

min = [0]
for value in arr:
    if value < min:
        min = value 
print(min)
```
## Exercise: 9
- Move one step to right 
  - Expected Output:[0, 1, 0, 0, 0]
```python
arr = [0 ,0, 1, 0, 0]
isFound = False
for i in range(len(arr)-1):
    if arr[i] == 1 and not isFound:
        arr[i] = 0
        arr[i-1] = 1
        isFound = True
print(arr)
```
## Exercise: 10
- Move one step to left 
  - Expected Output:[0, 1, 0, 0, 0] 
````python
arr = [0 ,0, 1, 0, 0]
isFound = False
for i in range(len(arr)-1):
    if arr[i] == 1 and not isFound:
        arr[i] = 0
        arr[i-1] = 1
        isFound = True
print(arr)
````
## Exercise: 11
-  find maximum number in the list
    - Output: 40
````python
arr = [10,40,20,4,3]
max = arr[0]
for value in arr:
    if value > max:
        max = value
print(max)
````

## Exercise: 12
- Sum of Rows in a 2D Array
- Output: 
````python
arr2D = [
    [1,2,3],
    [4,5,6],
    [7,8,9],
]
sum =0
arr = []
for i in range(len(arr2D)):
    for col in range(len(arr2D[row])):
        sum += arr2D[row][col]
    arr.append(sum)
    sum =0
print(arr)