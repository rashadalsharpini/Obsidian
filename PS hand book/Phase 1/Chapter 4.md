### map
is generalized array that consists of key-value-pairs where the key
in the ordinary array is consecutive 1,2,3,....,n-1, the key in 
the map doesn't have to consecutive values it can be of any data type.
the c++ standard library contains two types the structured map
depends on a balanced binary tree with an access time of O(logn) time,
while the structured unordered_map uses hashing with an access time of O(1) time on average.

```cpp
void solve(){
	int n;cin>>n;
	vi v(n);
	map<int, int> count;
	for(int i=0;i<n;++i){
		cin>>v[i];
		count[v[i]]++;
	}
}
// v = [1, 1, 1, 1, 2, 2, 2]
// count = [{1, 4}, {2, 3}]
```