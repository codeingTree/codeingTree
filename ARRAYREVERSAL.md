#include <iostream> 
#include<iomanip>
using namespace std;
void ReverseArray(int n,int arr[]){
    int start=0;
    int end=n-1;
    while(start<=end)
    {   
        swap(arr[start],arr[end]);
        start++;
        end--;
    }
}
int main()
{
int n;
cin>>n;
int arr[n];
for(int i=0;i<n;i++)
cin>>arr[i];
ReverseArray(n,arr);
for(int i=0;i<n;i++)
cout<<arr[i]<<" ";
return 0;
}
