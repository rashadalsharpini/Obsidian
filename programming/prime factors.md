```cpp
#include <bits/stdc++.h>  
using namespace std;  
  
vector<int> primeFactors(int n) {  
    vector<int> factors;  
  
    // Check for the number of 2s that divide n  
    while (n % 2 == 0) {  
        factors.push_back(2);  
        n /= 2;  
    }  
  
    // Check for odd factors from 3 onwards  
    for (int i = 3; i <= sqrt(n); i += 2) {  
        while (n % i == 0) {  
            factors.push_back(i);  
            n /= i;  
        }  
    }  
  
    // If n is a prime number greater than 2  
    if (n > 2) {  
        factors.push_back(n);  
    }  
  
    return factors;  
}  
  
int main() {  
    int n = 52;  
    vector<int> factors = primeFactors(n);  
	 
    cout << "Prime factors of " << n << ": ";  
    for (int factor : factors) {  
        cout << factor << " ";  
    }  
    cout << endl;  
	//Prime factors of 52: 2 2 13
    return 0;  
}
```
