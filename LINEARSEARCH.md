//>>>>>>>>>>>> SEARCH AN ELEMENT OF A USER GIVEN ARRAY,IF IT IS PRESENT IN THE ARRAY PRINT THE INDEX OR PRINT -1 <<<<<<<<
#include <iostream> 
#include<iomanip>
using namespace std;
int LinearSearch(int n,int arr[],int key){
    for(int i=0;i<n;i++)
    if(arr[i]==key)
    return i;
    return -1;
}
int main()
{
    int n,k;
    cin>>n>>k;
    int arr[n];
    for(int i=0;i<n;i++)
    cin>>arr[i];
    cout<<LinearSearch(n,arr,k);
return 0;
}  
