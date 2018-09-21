# Calculator-Pt1
Initial basic calculator code.


//  iostream uses the objects cin , cout , cerr , and clog for sending data to and from the standard streams input, output, error 
#include <iostream>

// A namespace is a form of scope in C++ that holds its own definitions for variables, functions, etc.
using namespace std;

// Begin main function
int main(){
    
    // Define character 'Operator' and Floating point integers num1 & num2
    char Operator;
    float num1, num2;

    // Enter operators 
    cout << "Enter operator +, -, *, or / : ";
    cin >> Operator;

    // Enter Values
    cout << "Enter two numbers: ";
    cin >> num1 >> num2;

    cout << num1 << Operator << num2 << endl;
    
    // Switch statements are essentially long 'if' statements the can branch multiple ways based on the selection of, in this case, the operator
    switch(Operator){
        
        // Addition case
        case '+':
        cout << num1 + num2;
        break;

        // Subtraction case
        case '-':
        cout << num1 - num2;
        break;

        // Multiplication case
        case '*':
        cout << num1 * num2;
        break;

        // Division case
        case '/':
        cout << num1/num2;
        break;

        // Default in case the user doesn't select a given operator
        default:
            //If the operator is not one of the given operators
            cout << "Error! operator is not correct";
            break;

    }
    // Pauses so the program doesn't exit before being executed
    system("pause");
    // Returns value to main
    return 0;
}
