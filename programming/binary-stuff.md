#Python 
```py
print(int('100', 2))  # binary to decimal
print(int(bin(4)[2:]))  # decimal to binary
```

```py
# shift Right  N/2
print(10 >> 1)  # 1010 become 101 = 5  
print(10 >> 2)  # 1010 become 10 = 2  
print(10 >> 3)  # 1010 become 1 = 1  
print(10 >> 4)  # 1010 become  = 0
# shift Left   N*2
print(10 << 1)  # 1010 become 10100 = 20
print(10 << 2)  # 1010 become 101000 = 40
print(10 << 3)  # 1010 become 101000 = 80
print(10 << 4)  # 1010 become 1010000 = 160

```

```py
print(2 & 4)
"""
2 0010 and
4 0100
0 0000
"""
print(2 | 4)
"""
2 0010 or
4 0100
6 0110
"""
print(3 ^ 4)
"""
3 0011 Xor
5 0101
6 0110
"""
```

```md
  5 ==> 0101
& 1 ==> 0001
True which means odd
  4 ==> 0100
& 1 ==> 0001
False which means even
it all debends on the last postion from the right
if it's 1 then it's odd
else it's even
```

```py
def decToBin(n):  
    a = []  
    for i in range(n):  
        a.append(n % 2)  
        n //= 2  
        # the problem is the loop
    a.reverse()  
    bing = 0  
    for i in range(len(a)):  
        if a[i] == 1:  
            bing = a[i:]  
            break  
    return bing  
  
  
if __name__ == "__main__":  
    y = 341341229080982343290815643985270348957  
    x = decToBin(y)  # Doesn't even print my laptop crash before the answer
    print(*x)  
    print(bin(y)[2:]) # way faster, almost instant
```

```py
for i in range(100):  
    print(~i, i)
```

```py
a = [0, 1, 2, 3]  
for i in range(1 << len(a)):  
    msk = i  
    j = 0  
    while msk:  
        if msk & 1:  
            print(a[j], end=' ')  
        j += 1  
        msk >>= 1  
    print()
```