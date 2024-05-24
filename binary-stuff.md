```py
print(int('100', 2))  # binary to decimal
print(int(bin(4)[2:]))  # decimal to binary
```

```py
print(10 >> 1)  # 1010 become 101 = 5  
print(10 >> 2)  # 1010 become 10 = 2  
print(10 >> 3)  # 1010 become 1 = 1  
print(10 >> 4)  # 1010 become  = 0
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