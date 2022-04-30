#include <iostream>
#include <iomanip>
using namespace std;
// BINARY SEARCH Function
int BinarySearch(int arr[], int n, int k)
{
    int start = 0;
    int end = n - 1;
    int mid = start + (end - start) / 2;
    while (start <= end)
    {
        if (arr[mid] == k)
            return mid;
        else if (k > arr[mid])
            start = mid + 1;
        else if (k < arr[mid])
            end = mid - 1;
        mid = start + (end - start) / 2;
    }
    return -1;
}

int main()
{
    int n, k;
    cin >> n >> k;
    int arr[n];
    for (int i = 0; i < n; i++)
        cin >> arr[i];
    cout << BinarySearch(arr, n, k);
    return 0;
}
