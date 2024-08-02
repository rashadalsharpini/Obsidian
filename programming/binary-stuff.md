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

### Sub Sequences - complete search
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

```cpp
#include <iostream>
#include <vector>
using namespace std;
int main() {
    vector<int> a = {0, 1, 2, 3};
    int n = a.size();
    
    for (int i = 0; i < (1 << n); ++i) {
        int msk = i;
        int j = 0;
        
        while (msk) {
            if (msk & 1) {
                cout << a[j] << " ";
            }
            j++;
            msk >>= 1;
        }
        cout << endl;
    }

    return 0;
}

```

```py
def get_bit(n, i):  
    if int(bin(n & (1 << i))[2:]) != 0:  
        return 1  
    return 0  
  
  
def set_bit(n, i, value):  
    if value:  
        return n | (1 << i)  
    else:  
        return n & ~(1 << i)  
  
  
def flip_bit(n, i):  
    return n ^ (1 << i)
```

### Prefix Xor
```py
n = int(input())  
a = list(map(int, input().split()))  
prefix = [0]*(n+5)  
for i in range(n):  
    prefix[i+1] = a[i] ^ prefix[i]  
l, r = map(int, input().split())  
print(prefix[r] ^ prefix[l - 1])
```