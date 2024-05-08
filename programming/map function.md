Map  - map(function, iterable)
	- Returns an iterator that applies function to every item of iterable
---
```py
def make_even(num):
	if num % 2 == 1:
		return num + 1
	else
		return num


x = [551, 641, 891, 122, 453, 223, 234, 343, 562, 115, 554, 111, 679, 516]
y = list(map(make_even, x))
print(y)
# the long way
ys = []
for num in x:
	ys.append(make_even(num))
print(ys)
# or you can use this
yx = [make_even(num) for num in x]
print(yx)
```
