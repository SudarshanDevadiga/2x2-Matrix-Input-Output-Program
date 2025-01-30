# 2x2 Matrix Input/Output Program

A simple C++ program that takes a 2x2 matrix as input from the user and then displays the entered matrix.

## Description

This program demonstrates how to use nested loops to take input from the user and store it in a 2D array (matrix), and then how to display the matrix in a user-friendly format. It's a good example of basic matrix handling in C++.

### Key Features
- User input for matrix elements
- Nested loops for matrix traversal
- Clear output formatting

## Code Structure

```cpp
#include <iostream>
using namespace std;

int main() {
    int matrix[2][2];
    cout << "Enter the elements of the 2x2 matrix:" << endl;
    // Taking input for the matrix
    for(int i=0; i<2; i++) {
        for(int j=0; j<2; j++) {
            cout << "Element [" << i << "][" << j << "]: ";
            cin >> matrix[i][j];
        }
    }
    // Displaying the matrix
    cout << "The 2x2 matrix is:" << endl;
    for(int i=0; i<2; i++) {
        for(int j=0; j<2; j++) {
            cout << matrix[i][j] << " ";
        }
        cout << endl;
    }
    return 0;
}
