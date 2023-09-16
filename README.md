from random import random
N = 10 
arr = [0] * N
for i in range(N):
    arr[i] = int(random() * 50)
print(arr)
for i in range(N-1):
    for j in range(i+1, N):
        if arr[i] == arr[j]:
            print("Есть одинаковые")
            quit()
print("Все элементы уникальны")
setarr = set(arr)
if len(arr) == len(setarr):
    print("Все элементы уникальны")
else:
    print("Есть одинаковые")
from random import randrange
 
N = 10
arr = [randrange(50) for i in range(N)]
print(*arr)
 
for item in arr:
    if arr.count(item) > 1:
        print("Есть одинаковые")
        break
else:
    print("Все элементы уникальны")
from random import randrange
 
N = 10
arr = [randrange(50) for i in range(N)]
print(*arr)
 
for item in arr:
    count = arr.count(item)
    if count > 1:
        print(f"Элемент {item} встречается {count} раз")
from random import randrange
 
N = 10
arr = [randrange(50) for i in range(N)]
print(*arr)
 
setarr = set(arr)
 
for item in setarr:
    count = arr.count(item)
    if count > 1:
