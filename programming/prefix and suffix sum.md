```cpp
void solve() {  
    int n;cin>>n;  
    vi v(n);cin>>v;  
    vi prefixsum(n + 1, 0);  
    
    for(int i = 1;i < n + 1;++i)  
        prefixsum[i] = prefixsum[i - 1] + v[i - 1];  
    
    cout<<prefixsum<<endl;  
    vi suffixsum(n, 0);  
    suffixsum[n - 1] = v[n - 1];  
    
    for(int i = n - 2; i>=0;--i)  
        suffixsum[i] = suffixsum[i+1] + v[i];  
    cout<<suffixsum<<endl;  
}
```