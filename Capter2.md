4. 倒三角形

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
5. 统计

```
#define LOCAL
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
    int n,m;
    cin >> n;
    int a[n];
    for(int i=0;i<n;i++){
        cin >> a[i];
    }
    cin >> m;
    int ccount=0;
    for(int j=0;j<n;j++){
        if(a[j]<m){
            ccount++;
        }
    }
    cout << ccount <<"\n";
    return 0;
}

```

6. 调和级数

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
    double h=0;
    cin >> n;
    for(int i=1;i<=n;i++){
        h += 1.0/i;
    }
    cout.setf(ios::showpoint); //设置为始终输出小数点后的数字，就是说 a = 3，它也输出 3.00000 这样
    cout.precision(3);
    cout.setf(ios::fixed); //设置为小数位始终有 6 位，没有这个的话就会像上面那个代码那样固定的不是小数点后面的数字了。
    cout << h <<"\n";
    return 0;
}

```

7. 

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
//    int n;
    double h=0;
//    cin >> n;
    for(int i=0;i<=500000;i++){
        if(i%2 == 1){
            h -= 1.0/(2*i+1);
        }else{
            h += 1.0/(2*i+1);
        }
    }
//    cout.setf(ios::showpoint); //设置为始终输出小数点后的数字，就是说 a = 3，它也输出 3.00000 这样
//    cout.precision(3);
//    cout.setf(ios::fixed); //设置为小数位始终有 6 位，没有这个的话就会像上面那个代码那样固定的不是小数点后面的数字了。
    cout << h <<"\n";
    return 0;
}

```
8. 子序列的和

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
    int n,m;
    double h=0;
    cin >> n >> m;
    for(int i=n;i <= m;i++){
        h += 1.0/i/i;
    }
    cout.setf(ios::showpoint); //设置为始终输出小数点后的数字，就是说 a = 3，它也输出 3.00000 这样
    cout.precision(5);
    cout.setf(ios::fixed); //设置为小数位始终有 6 位，没有这个的话就会像上面那个代码那样固定的不是小数点后面的数字了。
    cout << h <<"\n";
    return 0;
}

```

9. 分数化小数

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
//    int n,m;
//    double h=0;
//    cin >> n >> m;
//    for(int i=n;i <= m;i++){
//        h += 1.0/i/i;
//    }
//    cout.setf(ios::showpoint); //设置为始终输出小数点后的数字，就是说 a = 3，它也输出 3.00000 这样
//    cout.precision(5);
//    cout.setf(ios::fixed); //设置为小数位始终有 6 位，没有这个的话就会像上面那个代码那样固定的不是小数点后面的数字了。
//    cout << h <<"\n";
    int a,b,c;
    cin >> a >> b >> c;
//    int d=a;
cout << a/b << ".";
        a=a%b*10;
    for(int i=1;i<c;i++){
        cout << a/b;
        a=a%b*10;
    }
    int ee= a/b;
    a=a%b*10;
    if(a/b>=5){
        cout << ee+1;
    }else{
    cout << ee;
    }

    cout << "\n";
    return 0;
}

```

10. 
