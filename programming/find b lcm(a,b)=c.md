```cpp
#include <iostream>  
#include <vector>  
#include <algorithm>  
#include <numeric> // for gcd  
#include <cmath> // for sqrt  
using namespace std;  
vector<long long> find_b(long long a, long long c) {  
    vector<long long> possible_b_values;  
    long long sqrt_a = sqrt(a);  
  
    for (long long d = 1; d <= sqrt_a; ++d) {  
        if (a % d == 0) {  
            long long divisor1 = d;  
            long long divisor2 = a / d;  
            long long b1 = (c * divisor1) / a;  
            if ((c * divisor1) % a == 0 && gcd(a, b1) == divisor1) {  
                possible_b_values.push_back(b1);  
            }  
            if (divisor1 != divisor2) {  
                long long b2 = (c * divisor2) / a;  
                if ((c * divisor2) % a == 0 && gcd(a, b2) == divisor2) {  
                    possible_b_values.push_back(b2);  
                }  
            }  
        }  
    }  
    return possible_b_values;  
}  
void solve() {  
    long long a, c;  
    cin >> a >> c;  
    vector<long long> result = find_b(a, c);  
    if (result.empty()) {  
        cout << -1 << endl;  
    } else {         
	    cout << *min_element(result.begin(), result.end()) << endl;  
    }  
}
```