[A. Problem Generator](https://codeforces.com/contest/1980/problem/A)
[B. Choosing Cubes](https://codeforces.com/contest/1980/problem/B)
counting in python
count list string go a head
and it returns a dictionary
```py
from collections import Counter


a = [4, 2, 3, 2, 2, 4, 5, 6]
count = Counter(a)[2]
freq_a = Counter(a)
print(count)
print(freq_a)
```
![[Pasted image 20240605223838.png]]
![[Pasted image 20240605223940.png]]

```py
from collections import Counter


if __name__ == '__main__':
	a = list(map(int, bin(4312)[2:]))
	count = Counter(a)
	print(count)
	# Counting '1's directly from the list
	count_of_ones = count[1]
	print(count_of_ones)
	# Using Counter on the string version of `a`
	a_str = ''.join(map(str, a))
	count_str = Counter(a_str)
	most_common_char = count_str.most_common(1) # Get the most common character
	print(most_common_char) # [('1', count)]
```