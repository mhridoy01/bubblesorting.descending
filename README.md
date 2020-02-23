# bubblesorting.descending

#include<bits/stdc++.h>
using namespace std;
int main()
{
    int arr[100],n;
    scanf("%d",&n);
    for(int i=1;i<=n;i++)
        scanf("%d",&arr[i]);
    for(int i=1;i<=n-1;i++)
    {
        for(int j=1;j<=n-i;j++)
        {
            if(arr[j]<arr[j+1])
                swap(arr[j],arr[j+1]);
        }
    }
    for(int i=1;i<=n;i++)
        printf("%d ",arr[i]);
    return 0;
}

