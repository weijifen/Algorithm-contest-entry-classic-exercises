4. 

```
//#define LOCAL
#include <iostream>
#include <cstdio>
#include <stdio.h>
#include <stdlib.h>
#include<time.h>

using namespace std;

int main()
{
    #ifdef LOCAL
    freopen("data.in","r",stdin);
    freopen("data.out","w",stdout);
    #endif // LOCAL
    int n;
    cin >> n;
    for(int i=1;i<=n;i++){
        for(int j=1;j<=i-1;j++){
            cout << " ";
        }
        for(int k=1;k<=2*n-2*i+1;k++){
            cout << "#";
        }
        cout << "\n";
    }
    return 0;
}

```
