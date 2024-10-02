#include <iostream>
using namespace std;

int main() {
    char operation;
    float num1, num2;

    // Displaying options to the user
    cout << "Simple Calculator" << endl;
    cout << "Choose an operation (+, -, *, /): ";
    cin >> operation;

    // Asking for input numbers
    cout << "Enter two numbers: ";
    cin >> num1 >> num2;

    // Performing the calculation based on the chosen operation
    switch (operation) {
        case '+':
            cout << "Result: " << num1 + num2 << endl;
            break;
        case '-':
            cout << "Result: " << num1 - num2 << endl;
            break;
        case '*':
            cout << "Result: " << num1 * num2 << endl;
            break;
        case '/':
            if (num2 != 0)
                cout << "Result: " << num1 / num2 << endl;
            else
                cout << "Error: Division by zero is not allowed!" << endl;
            break;
        default:
            cout << "Error: Invalid operation!" << endl;
            break;
    }

    return 0;
}
