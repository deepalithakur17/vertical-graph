# vertical-graph
Vertical Graph in C++ 

#include<bits/stdc++.h>
using namespace std;

int main()
{
    int n;
    cout<<"enter the number of elements in a array :";
    cin>>n;
    int i=0;
    int arr[n];
    int max=0;
    while(i<n)
    {
        cin>>arr[i];
        i++;
    }
    
    for(int i=0;i<n;i++)
    {
        if(arr[i]>max)
        {
            max=arr[i];
        }
    }
    for(int i=max;i>=1;i--)
    {
        for(int j=0;j<n;j++)
        {
            if(i<=arr[j])
            {
                cout<<"* ";
            }
            else
            {
                cout<<"  ";
            }
        }
        cout<<endl;
    }

}
