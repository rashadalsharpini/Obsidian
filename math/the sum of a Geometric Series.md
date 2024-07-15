3 6 12 24 48 96
r = 2
$$an = a1.r^n-1$$
$$a4 = a1 . r^3$$
$$24 = 3 . 2^3$$
3+6+12+24+48+96 = s6 = 189
$$Sn = (a1[1-r^n])/(1 - r)$$
$$S6 = (3[1-2^6])/(1-2) = 189$$
$$S infinite = a1/1-r$$ converges

$$1/2 + 2/4 + 3/8 + 4/16 + 5/32$$
$$2^r+1 - 2 - r$$


```py
MOD = 10**9 + 7


def fast_power(a, b):
    res = 1
    while b:
        if b & 1:
            res *= a % MOD
        a *= a % MOD
        b >>= 1
    return res

%
def solve():
    r = int(input())
    ans = (fast_power(2, r + 1) - 2 - r) % MOD
    if ans < 0:
        ans += MOD
    print(ans)

```