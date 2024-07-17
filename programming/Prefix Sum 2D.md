```cpp
void solve() {  
    int n, m, q;  
    cin >> n >> m >> q;  
    vector<vector<ll>> a(n, vector<ll>(m));  
    for (int i = 0; i < n; ++i)  
        for (int j = 0; j < m; ++j)  
            cin >> a[i][j];  
    ll x1,x2,y1,y2;vector<vector<ll>> ps(n + 1, vector<ll>(m + 1, 0));  
    for (ll i = 1; i <= n; ++i)  
        for (ll j = 1; j <= m; ++j)  
            ps[i][j] = a[i - 1][j - 1] + ps[i - 1][j] + ps[i][j - 1] - ps[i - 1][j - 1];  
    for(ll i = 0;i<q;++i) {  
        cin>>x1>>y1>>x2>>y2;  
        ll sum_rect = ps[x2][y2] - ps[x1 - 1][y2] - ps[x2][y1 - 1] + ps[x1 - 1][y1 - 1];  
        cout<<sum_rect<<endl;  
    }  
  
}
```