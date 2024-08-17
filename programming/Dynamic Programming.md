![[Concept.excalidraw]]



## example
### $O(2^n)$
```cpp
int fib(int n) {  
    if(n<=1)  
        return n;  
    return fib(n - 2) + fib(n - 1);  
}
```

### $O(n)$ - Tabulation - iterative
```cpp
int fibb(int n) {  
    vi ff(n + 1, -1);  
    if(n<=1)  
        return n;  
    ff[0] = 0, ff[1] = 1;  
    for (int i = 2;i <= n;++i)  
        ff[i] = ff[i -2]+ff[i-1];  
    return ff[n];  
}
```

### $O(n)$ - Memorization - recursive
```cpp
#include <vector>
int fibbb(int n, vi& memo) {  
    if (n <= 1)  
        return n;  
    if (memo[n] != -1)  
        return memo[n];  
    memo[n] = fibbb(n - 1, memo) + fibbb(n - 2, memo);  
    return memo[n];  
}
```
