# c++code for Fibonacci Series 
C++ code 
#include <iostream>
using namespace std;

int main() {
int n;
cin >> n;

int a = 0, b = 1;

for (int i = 2; i < n; i++) {
    int next = a + b;
    a = b;
    b = next;
}

cout << a << " " << b;

return 0;

} 
# c++code for Factorial Recursion 

#include <iostream>
using namespace std;

int fact(int n);

int main() {
int n, factorial;

cout << "Enter value: ";
cin >> n;

factorial = fact(n);

cout << "Factorial of " << n << " is " << factorial;

return 0;

}

int fact(int n) {
if (n == 0 || n == 1) {
return 1;
}
else {
return n * fact(n - 1);
}
} 
# c++code for Stack Push 
void push()
{
    int x;

    if (top == size - 1)
    {
        cout << "Stack Overflow\n";
    }
    else
    {
        cout << "Enter element: ";
        cin >> x;
        top++;
        stack[top] = x;
    }
} 
# c++code for Stack Pop
void pop()
{
    if (top == -1)
    {
        cout << "Stack Underflow\n";
    }
    else
    {
        cout << "Popped element: " << stack[top] << endl;
        top--;
    }
}
