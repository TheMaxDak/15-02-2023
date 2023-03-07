# Задание 1
```
arr = []
imax = 0
jmax = 0
imin = 0
jmin = 0
x = int(input("размер = "))
for i in range(x):
    arr.append([])
    for j in range(x):
        n = input(f"A[{i}][{j}] = ")
        arr[i].append(n)
min = arr[0][0]
max = arr[0][0]
for i in range(x):
    print()
    for j in range(x):
        print(" ",arr[i][j],end = ' ')
for i in range(x):
    print()
    for j in range(x):
        if(arr[i][j] > max):
            max = arr[i][j]
            imax = i
            jmax = j
        if(arr[i][j] < min):
            min = arr[i][j]
            imin = i
            jmin = j
print("минимальный =", min,"   i =", imin,"j =", jmin)
print("максимальный = ", max,"   i =",imax,"j =", jmax)
```

# Задание 2
```

import random

m, n = 2, 2
matrix_2 = [[random.randint(-100, 100)
for _ in range(n)]
for _ in range(m)]
print(matrix_2)
print(max(matrix_2, key=sum))

matrix_2 = [list(filter(lambda x: x % 2 == 0 and x > 0, matrix))
for matrix in matrix_2]
print(matrix_2)

min_matrix = [min(matrix)
for matrix in matrix_2
if matrix]
print(min_matrix)

max_matrix = [max(matrix)
for matrix in matrix_2
if matrix]
print(max_matrix)

print(min(min_matrix)) \
if min_matrix \
else print('В матрице нет четных элементов больше нуля')
print(max(max_matrix)) \
if max_matrix \
else print('В матрице нет четных элементов больше нуля')
```

# Задание 11
```

def wtf(x,y,z):
    if x == z or x ==y or z ==y:
        return True
    else:
        return False
        
print(wtf(1,2,2))
```

# Задание 14
```

def function():
    list = []
    str1 = input()
    str2 = input()
    list.append(str1 + str2)
    print(list)
function()
```

# Задание 15
```

def function():
    a = {1:'peanut', 2:'butter', 3:'jelly', 4:'time'}
    b = {5:'fish', 6:'chips'} 
    x = a|b
    print(x)
function()
```

# Задание 16
```

def factorial(number):
    if number == 1:
        return number
    else:
        return number * factorial(number - 1)

print(factorial(int(input('Введите число: '))))
```
# Задание 17
```

def function():
    l = input()
    for i in l:
        print(i)
function()
```

# Задание 18
```

def function():
    a = []
    n = int(input())
    for i in range(n):
        x = int(input())
        a.append(x)
    for z in a:
        print(z)
function()
```
