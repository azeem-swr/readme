### 1. **What are the three types of programming languages? Provide examples.**

**Answer:**

- **Machine Language:** Consists of binary digits (1s and 0s) directly understood by the computer. Example: `00101010 000000000001 000000000010`.
- **Assembly Language:** Uses mnemonics for instructions, translated to machine code by an assembler. Example: `LOAD BASEPAY`.
- **High-Level Language:** Uses English-like statements. Example: `grossPay = basePay + overTimePay`.

---

### 2. **What is structured programming, and what are its key features?**

**Answer:**

- **Definition:** Structured programming divides a problem into smaller subproblems using a top-down or bottom-up approach.
- **Features:** Stepwise refinement and modular programming.

---

### 3. **What is object-oriented programming (OOP), and what are its key characteristics?**

**Answer:**

- **Definition:** OOP involves identifying components called objects and determining their interactions.
- **Key Characteristics:**
  - Objects combine data and operations into a single unit.
  - Focus on representing data in memory and manipulating it.

---

### 4. **What are tokens in C++? List examples.**

**Answer:**

- **Definition:** Tokens are the smallest individual units of a program that have meaning.
- **Examples:**
  - Special symbols: `+`, `*`, `/`, `<=`.
  - Reserved words: `int`, `float`.
  - Identifiers: User-defined names like `myVariable`.

---

### 5. **What are the rules for defining identifiers in C++?**

**Answer:**

- Must start with a letter or underscore.
- Can include letters, digits, and underscores but no spaces or special characters.
- Cannot be a reserved keyword.

---

### 6. **What are the data types in C++? Give examples of each.**

**Answer:**

- **Primitive Data Types:** `int`, `float`, `char`, `bool`.
- **Structured Data Types:** Arrays, structures.
- **Pointer Types:** Stores memory addresses.

---

### 7. **Explain the difference between pre-increment (++i) and post-increment (i++).**

**Answer:**

- **Pre-Increment:** Increases the value first, then uses it in the expression. Example: `j = ++i;` (i and j both increase).
- **Post-Increment:** Uses the value first, then increases it. Example: `j = i++;` (j gets old value, i increases later).

---

### 8. **What are the differences between **********`** and **`********** in C++?**

**Answer:**

- **cin:** Stops input at whitespace, used for individual words or numbers.
- **getline():** Reads an entire line, including spaces, until a newline is encountered.

---

### 9. **What are conditional statements in C++? Provide examples.**

**Answer:**

- **Definition:** Statements that execute based on a condition being true or false.
- **Examples:**
  - `if-else`:
    ```cpp
    if (age > 18) cout << "Eligible to vote.";
    else cout << "Not eligible.";
    ```
  - `switch-case`:
    ```cpp
    switch (grade) {
      case 'A': cout << "Excellent"; break;
      default: cout << "Invalid grade.";
    }
    ```

---

### 10. **Explain the concept of loops in C++ with examples.**

**Answer:**

- **Types:**
  - \`\`\*\* loop:\*\* Executes while a condition is true.
    ```cpp
    while (count < 5) { cout << count; count++; }
    ```
  - \`\`\*\* loop:\*\* Combines initialization, condition, and update.
    ```cpp
    for (int i = 0; i < 5; i++) { cout << i; }
    ```
  - \`\`\*\* loop:\*\* Executes the loop body at least once.
    ```cpp
    do { cout << count; } while (count < 5);
    ```

---

### 11. **What are relational operators in C++? Provide examples.**

**Answer:**

- **Definition:** Compare two values and return a boolean result.
- **Examples:**
  - `==` (equal to): `5 == 5` → true.
  - `<` (less than): `3 < 7` → true.

---

### 12. **What are logical operators in C++? Explain with examples.**

**Answer:**

- **Operators:**
  - `&&` (AND): Both conditions must be true.
  - `||` (OR): At least one condition must be true.
  - `!` (NOT): Reverses the condition.
- **Example:**
  ```cpp
  if (x > 0 && y < 10) cout << "Valid range.";
  ```

---

### 13. **What is the purpose of \`\` directives in C++?"**

**Answer:**

- Used to include libraries required for a program.
- Example: `#include <iostream>` provides `cin` and `cout`.

---

### 14. **What are the differences between compilers and interpreters?**

**Answer:**

- **Compiler:** Translates the entire program into machine code before execution.
- **Interpreter:** Translates and executes code line by line.

---

### 15. **Explain file handling in C++ with basic operations.**

**Answer:**

- **Include Header:** `#include <fstream>`.
- **Classes:**
  - `ofstream`: For writing to a file.
  - `ifstream`: For reading from a file.
- **Example:**
  ```cpp
  ofstream file("example.txt");
  file << "Hello World!";
  file.close();
  ```

---

### 16. **What is the difference between value-returning functions and void functions in C++?**

**Answer:**

- **Value-Returning Functions:** Return a value using the `return` statement. Example:
  ```cpp
  int add(int a, int b) {
      return a + b;
  }
  ```
- **Void Functions:** Perform an action but do not return a value. Example:
  ```cpp
  void printMessage() {
      cout << "Hello!";
  }
  ```

---

### 17. **How can arrays be initialized in C++? Provide examples.**

**Answer:**

- **Direct Initialization:**
  ```cpp
  int arr[3] = {1, 2, 3};
  ```
- **Using Loops:**
  ```cpp
  for (int i = 0; i < 3; i++) {
      arr[i] = i + 1;
  }
  ```

---

### 18. **What is the purpose of nested loops in C++? Provide an example.**

**Answer:**

- **Purpose:** Used to iterate over multi-dimensional data structures such as 2D arrays.
- **Example:**
  ```cpp
  for (int i = 0; i < 3; i++) {
      for (int j = 0; j < 3; j++) {
          cout << i << ", " << j << endl;
      }
  }
  ```

---

### 19. **What are the advantages of using functions in C++?**

**Answer:**

- Reusability: Functions can be reused multiple times.
- Modularity: Helps in dividing a program into smaller, manageable parts.
- Debugging: Easier to test and debug specific sections of code.
- Readability: Enhances the clarity of the program structure.

---

### 20. **What is the difference between "pass by value" and "pass by reference" in functions?**

**Answer:**

- **Pass by Value:** A copy of the actual parameter is passed. Modifications do not affect the original variable. Example:
  ```cpp
  void modify(int a) { a = 10; }
  ```
- **Pass by Reference:** The actual parameter is passed. Modifications affect the original variable. Example:
  ```cpp
  void modify(int &a) { a = 10; }
  ```

---

### 21. **Explain the concept of default arguments in C++ functions.**

**Answer:**

- Default arguments allow functions to be called without providing all the arguments explicitly.
- Example:
  ```cpp
  int sum(int a, int b = 5) { return a + b; }
  // sum(3) returns 8; sum(3, 7) returns 10.
  ```

---

### 22. What is exception handling in C++? Provide examples of \*\*, \*\*, and \`\`.

**Answer:**

- **Definition:** Exception handling is used to handle runtime errors and ensure the program runs smoothly without crashing.
- **Components:**
  - `try`: Block where the code is tested for exceptions.
  - `catch`: Block that handles the exception.
  - `throw`: Used to throw an exception.
- **Example:**
  ```cpp
  try {
      int denominator = 0;
      if (denominator == 0) throw "Division by zero error";
  } catch (const char* msg) {
      cout << msg;
  }
  ```

---

### 23. **What is the purpose of ********`ofstream`********, ********`ifstream`********, and ********`fstream`******** in C++?**

**Answer:**

- `ofstream`: Used to write data to files. Example:
  ```cpp
  ofstream file("example.txt");
  file << "Writing to a file.";
  file.close();
  ```
- `ifstream`: Used to read data from files. Example:
  ```cpp
  ifstream file("example.txt");
  string content;
  while (getline(file, content)) {
      cout << content;
  }
  file.close();
  ```
- \`\`**:** Used for both reading and writing data. Example:
  ```cpp
  fstream file("example.txt", ios::in | ios::out);
  file << "Read and write operations.";
  file.close();
  ```

---

### 24. **What is the difference between text files and binary files in C++?**

**Answer:**

- **Text Files:** Store data in human-readable text format. Example: `.txt` files.
- **Binary Files:** Store data in binary format, not human-readable. Example: `.bin` files.
- **Usage:** Binary files are faster and more efficient for storing large data, whereas text files are easier to debug and edit manually.

---

### 25. **How is file error handling implemented in C++?**

**Answer:**

- **Definition:** File error handling ensures that operations like opening, reading, or writing files are checked for success.
- **Example:**
  ```cpp
  ifstream file("example.txt");
  if (!file) {
      cout << "Error opening file.";
  } else {
      cout << "File opened successfully.";
  }
  file.close();
  ```

