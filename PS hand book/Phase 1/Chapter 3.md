### Comparison functions
it is possible to give an external comparison function to the sort as a call back function.
For example the following comparison function comp sorts strings primarily by length and secondly by alphabetical order.
```cpp
bool comp(string a, string b){
	if (a.size() != b.size()) return a.size < b.size();
	return a < b;
}
sort(v.begin(), v.end(), comp);
```

---
### binary search