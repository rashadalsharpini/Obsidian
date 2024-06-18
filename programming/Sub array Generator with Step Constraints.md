```py
n = int(input())  
a = list(map(int, input().split()))  
for i in range(n):  
    for j in range(i + 2, n + 1):        
	    print(a[i:j])
```

```md
4

2 4 1 7
  
[2,4],[2,4,1],[2,4,1,7],[4,1],[4,1,7],[1,7]
```