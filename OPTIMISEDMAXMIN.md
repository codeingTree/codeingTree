#include <iostream>
#include <iomanip>
#include <climits>
using namespace std;

int main()
{
  int n;
  cin >> n;
  int arr[n];
  for (int i = 0; i < n; i++)
    cin >> arr[i];
  int MaxElement = INT_MIN;
  int MinElement = INT_MAX;
  for (int i = 0; i < n; i++)
  {
    MaxElement = max(MaxElement, arr[i]);
    MinElement = min(MinElement, arr[i]);
  }
  cout << "Max is " << MaxElement << endl
       << "Min is " << MinElement << endl;
  return 0;
}
