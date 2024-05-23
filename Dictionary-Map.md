#Python 

```py
cnt = dict()  
triplet = (1, 2, 3)  
test = [tuple()] * 3  
test[0] = (0, 2, 3)  
test[1] = (1, 0, 3)  
test[2] = (1, 2, 0)  
ans = 0  
cnt = {  
    test[0]: 'rashad',  
    test[1]: 'yousef',  
    test[2]: 'sayd'  
}  
# print(test)  
for trip in test:  
    print(cnt.get(trip, 0))  # the second argument is returned if the key doesn't exist  
print(cnt)
```