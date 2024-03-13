```cpp
#include <iostream>  
using namespace std;  
int main() {  
    int size;cin>>size;  
    int arr1[size][size];  
    int arr2[size][size];  
    int arr3[size][size];  
    for (int i = 0; i < size; ++i) {  
        for (int j = 0; j < size; ++j) {  
            cin>>arr1[i][j];  
        }    }    for (int i = 0; i < size; ++i) {  
        for (int j = 0; j < size; ++j) {  
            cin>>arr2[i][j];  
        }    }    for (int i = 0; i < size; i++) {  
        for (int j = 0; j < size; j++) {  
            arr3[i][j] = 0;  
            for (int k = 0; k < size; k++) {  
                arr3[i][j] += arr1[i][k] * arr2[k][j];  
            }        }    }    for (int i = 0; i < size; ++i) {  
        for (int j = 0; j < size; ++j) {  
            cout<<arr3[i][j]<<" ";  
        }        cout<<endl;  
    }    return 0;  
}  
/*  
 * DECLARE size (integer)READ size  
  
// Initialize matrices with size x size dimensions  
DECLARE arr1 (2D array of integers, size x size)  
DECLARE arr2 (2D array of integers, size x size)  
DECLARE arr3 (2D array of integers, size x size)  
  
// Input elements for arr1  
FOR i = 0 TO size - 1 DO  
  FOR j = 0 TO size - 1 DO    READ arr1[i][j]  ENDFORENDFOR  
  
// Input elements for arr2  
FOR i = 0 TO size - 1 DO  
  FOR j = 0 TO size - 1 DO    READ arr2[i][j]  ENDFORENDFOR  
  
// Perform matrix multiplication and store result in arr3  
FOR i = 0 TO size - 1 DO  
  FOR j = 0 TO size - 1 DO    arr3[i][j] = 0 (initialize to 0 for summation)    FOR k = 0 TO size - 1 DO      arr3[i][j] = arr3[i][j] + (arr1[i][k] * arr2[k][j]) (dot product)    ENDFOR  ENDFORENDFOR  
  
// Print the resulting matrix arr3  
FOR i = 0 TO size - 1 DO  
  FOR j = 0 TO size - 1 DO    PRINT arr3[i][j]  PRINT newlineENDFOR  
 */
```
---
====>>>O(n^3)