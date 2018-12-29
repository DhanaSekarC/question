#include <iostream>
using namespace std;

int main() {
int t;
cin>>t;

while(t--)
{
int n;
cin>>n;

int a[n];
    
    for(int i=0;i<n;i++)
    cin>>a[i];
    
    int max1=a[0];
    int min1=a[0];
    for(int i=1;i<n;i++)
    {
        if((a[i]+i)>max1)
        max1=a[i]+i;
        else
            {if((a[i]+i)<min1)
            min1=a[i]+i;
            }
    
    }

    int max2=a[0];
    int min2=a[0];
    for(int i=1;i<n;i++)
    {
        if((a[i]-i)>max2)
        max2=a[i]-i;
        else
            {if((a[i]-i)<min2)
            min2=a[i]-i;
            }
    
    }
    
if((max1-min1)>=(max2-min2))
cout<<(max1-min1)<<'\n';
else
cout<<(max2-min2)<<'\n';
    
    
}
}

