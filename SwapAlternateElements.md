#include <iostream> 
#include<iomanip>
using namespace std;
void SwapAlternativeElements(int n,int arr[]){
    for(int i=0;i<n;i+=2){
        if(i+1<n)
        swap(arr[i],arr[i+1]);
    }
}
int main()
{
int n;
cin>>n;
int arr[n];
for(int i=0;i<n;i++)
cin>>arr[i];
SwapAlternativeElements(n,arr);
for(int i=0;i<n;i++)
cout<<arr[i]<<" ";
return 0;
}
