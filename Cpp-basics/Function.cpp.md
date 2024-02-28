**Function Declaration and Definition**:

   - **Function Declaration**:

     ```cpp
     // Function declaration
     return_type function_name(parameter_type parameter1, parameter_type parameter2, ...);
     ```

     **Explanation**: A function declaration tells the compiler about a function's name, return type, and parameters.

   - **Function Definition**:

     ```cpp
     // Function definition
     return_type function_name(parameter_type parameter1, parameter_type parameter2, ...) {
         // Function body
         // Perform tasks here
         return result; // Return statement (if applicable)
     }
     ```

     **Explanation**: A function definition provides the actual implementation of the function. It includes the return type, function name, parameter list, and function body.

     **Example**:

     ```cpp
     #include <iostream>
     using namespace std;
     
     // Function declaration
     int add(int a, int b);
     
     int main() {
         int result = add(5, 3); // Function call
         cout << "Result: " << result << endl;
         return 0;
     }
     
     // Function definition
     int add(int a, int b) {
         return a + b;
     }
     ```

     **Output**:
     ```
     Result: 8
     ```

2. **Function Parameters**:

   - **Explanation**: Functions can have zero or more parameters. Parameters are variables declared in the function declaration and definition. They are used to pass values to the function.

   - **Example**:

     ```cpp
     #include <iostream>
     using namespace std;
     
     // Function declaration
     void greet(string name);
     
     int main() {
         greet("John");
         greet("Jane");
         return 0;
     }
     
     // Function definition
     void greet(string name) {
         cout << "Hello, " << name << "!" << endl;
     }
     ```

     **Output**:
     ```
     Hello, John!
     Hello, Jane!
     ```

3. **Return Type**:

   - **Explanation**: Functions may or may not return a value. If a function returns a value, the return type specifies the type of the value returned by the function. If a function does not return a value, its return type is `void`.

   - **Example**:

     ```cpp
     #include <iostream>
     using namespace std;
     
     // Function declaration
     int square(int num);
     
     int main() {
         int result = square(5);
         cout << "Square: " << result << endl;
         return 0;
     }
     
     // Function definition
     int square(int num) {
         return num * num;
     }
     ```

     **Output**:
     ```
     Square: 25
     ```

4. **Calling Functions**:

   - **Explanation**: To execute a function, you need to call it from another part of your code. You call a function by using its name followed by parentheses `()` and passing arguments (if any).

   - **Example**:

     ```cpp
     #include <iostream>
     using namespace std;
     
     // Function declaration
     void displayMessage();
     
     int main() {
         displayMessage(); // Function call
         return 0;
     }
     
     // Function definition
     void displayMessage() {
         cout << "Hello, World!" << endl;
     }
     ```

     **Output**:
     ```
     Hello, World!
     ```

5. **Function Overloading**:

   - **Explanation**: C++ supports function overloading, which allows you to have multiple functions with the same name but different parameter lists. The compiler determines which function to call based on the number and types of arguments provided.

   - **Example**:

     ```cpp
     #include <iostream>
     using namespace std;
     
     // Function declaration
     void print(int num);
     void print(double num);
     
     int main() {
         print(5);
         print(3.14);
         return 0;
     }
     
     // Function definition
     void print(int num) {
         cout << "Integer: " << num << endl;
     }
     
     // Function definition
     void print(double num) {
         cout << "Double: " << num << endl;
     }
     ```

     **Output**:
     ```
     Integer: 5
     Double: 3.14
     ```

