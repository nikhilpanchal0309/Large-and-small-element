#include <iostream>
using namespace std;

int main() {
    int a[5];

    cout << "Enter 5 elements: ";
    for (int i = 0; i < 5; i++) {
        cin >> a[i];
    }

    int large = a[0];
    int small = a[0];

    for (int i = 1; i < 5; i++) {
        if (a[i] > large)
            large = a[i];

        if (a[i] < small)
            small = a[i];
    }

    cout << "Largest element = " << large << endl;
    cout << "Smallest element = " << small;

    return 0;
}
