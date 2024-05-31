#Python
```py
myList = [int(input()) for _ in range(5)]  # entering the array
filtered_list = [x for x in myList if x != 0]  # filtering the array of zeros
print(myList, filtered_list)
```

```py
n, m, c = (lambda x: (int(x[0]), int(x[1]), x[2]))(input().split())  
s = []  
for i in range(n):  
    s.append(input())  
print(*s, sep='\n', end='')
```
