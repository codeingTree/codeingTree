#include <iostream>
#include <climits>
  //climits for INT_MAX & INT_MIN function use
#include <iomanip>
using namespace std;
  //MINIMUM ELEMENT OF THE ARRAY
int GetMax(int arr[], int n)
{
  int max = INT_MIN;
  for (int i = 0; i < n; i++)
  {
    if (arr[i] > max)
      max = arr[i];
  }
  return max;
}
  //MINIMUM ELEMENT OF THE ARRAY
int GetMin(int arr[], int n)
{
  int min = INT_MAX;
  for (int i = 0; i < n; i++)
  {
    if (arr[i] < min)
      min = arr[i];
  }
  return min;
}
int main()
{
  int n=5;
  
  int arr[n]={9,8,7,3,4};
  cout<<"Maximum element of the array is "<<GetMax(arr,n)<<endl;
  cout<<"Minimum element of the array is "<<GetMin(arr,n);
  return 0;
}
