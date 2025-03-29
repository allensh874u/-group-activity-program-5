# -group-activity-program-5
#include <iostream>
using namespace std;

// Function to input and display the user's name
void getUserName() {
    string name;
    cout << "Enter the name of the user: ";
    cin >> name;
    cout << "Hello " << name << endl;
}

// Function to ask for two numbers
void getNumbers(int &num1, int &num2) {
    cout << "Enter first number: ";
    cin >> num1;
    cout << "Enter second number: ";
    cin >> num2;
}

// Function to add two numbers
int addNumbers(int a, int b) {
    return a + b;
}

// Function to subtract the second number from the first number
int subtractNumbers(int a, int b) {
    return a - b;
}

// Function to multiply two numbers
int multiplyNumbers(int a, int b) {
    return a * b;
}

// Function to divide the first number by the second number
double divideNumbers(int a, int b) {
    if (b == 0) {
        cout << "Error: Division by zero!" << endl;
        return 0;
    }
    return (double)a / b;
}

// Function to get the modulus of the first number
int modulusNumber(int a, int b) {
    if (b == 0) {
        cout << "Error: Modulus by zero!" << endl;
        return 0;
    }
    return a % b;
}

int main() {
    getUserName();

    int num1, num2;
    getNumbers(num1, num2);

    cout << "The sum of two numbers is: " << addNumbers(num1, num2) << endl;
    cout << "The difference of two numbers is: " << subtractNumbers(num1, num2) << endl;
    cout << "The product of two numbers is: " << multiplyNumbers(num1, num2) << endl;
    cout << "The quotient of two numbers is: " << divideNumbers(num1, num2) << endl;
    cout << "The modulus of first number is: " << modulusNumber(num1, num2) << endl;

    return 0;
}
