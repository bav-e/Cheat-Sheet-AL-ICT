# **Final Plan for Lesson 9 Cheat Sheet: Algorithms & Python Programming**

### **The Goal**

To create a comprehensive, single-page reference sheet that covers the entire programming lifecycle, from abstract problem-solving to practical Python implementation. The content will be based on both the official syllabus and the provided practical guide to ensure it meets the A/L standard.

### **The Structure: "From Idea to Executable"**

The cheat sheet will be structured into four logical parts, following the natural progression of software development.

## **Content List for the Cheat Sheet**

### **Part 1: The "Thinking" Phase \- Problem Solving & Algorithms**

*This section covers the abstract concepts of how to approach and define a solution.*

* **Problem Solving Process:**  
  * A cycle: Define Problem \-\> Generate Ideas \-\> Evaluate & Select \-\> Implement & Evaluate.  
* **Design Methodologies:**  
  * Modularization (Decomposition): Breaking a big problem into smaller, logical sub-problems.  
  * Top-down design & Stepwise refinement.  
* **Structure Charts:** A visual representation of the modular breakdown of a system.  
* **Algorithms:**  
  * **Definition:** A finite sequence of well-defined instructions to solve a problem.  
  * **Representations:**  
    * **Flowcharts:** A diagrammatic representation. (Include key symbols: Terminator, Process, Input/Output, Decision, Connector).  
    * **Pseudo-code:** A high-level, human-readable description. (Include structure for Begin/End, Read/Display, If/Else/Endif).  
  * **Core Constructs:** Sequence, Selection, Repetition (Iteration/Looping).  
* **Verification:** Hand Trace: Manually stepping through an algorithm to check for errors.

### **Part 2: The "Setup" Phase \- Programming Concepts & Environment**

*This section covers the background knowledge needed before writing code.*

* **Programming Paradigms (with sub-categories):**  
  * Imperative: Describes *how* to get a result.  
    * Sub-types: Procedural (e.g., C), Object-Oriented (e.g., Java), Parallel.  
  * Declarative: Describes *what* result you want.  
    * Sub-types: Logic (e.g., Prolog), Functional (e.g., Lisp), Database (e.g., SQL).  
* **Program Translation:**  
  * Source Code (human-readable) vs. Object Code (machine-readable).  
  * **Language Hierarchy:** A pyramid showing Hardware \-\> Machine \-\> Assembly \-\> High-level.  
  * **Translators:**  
    * Compiler: Translates the *entire* source code at once.  
    * Interpreter: Translates and executes *line-by-line*.  
    * Hybrid Approach: Combines both (like Python).  
  * Linker: Connects user code with standard library functions.  
* **IDE (Integrated Development Environment):**  
  * A software suite combining an Editor, Compiler/Interpreter, and a Debugger.

### **Part 3: The "Coding" Phase \- Python Core Syntax**

*This section provides a quick reference for Python's fundamental syntax, based on the practical guide.*

* **Basic Structure:** Comments (\#), and the importance of Indentation for defining scope.  
* **Variables & Data Types:**  
  * Variable: A named storage location. No explicit declaration command needed.  
  * **Primitive Data Types:** int, float, str, bool.  
  * **Type Casting:** Using int(), float(), str() to convert between types.  
* **Operators & Precedence:**  
  * **Categories:** Arithmetic (+, \-, \*, /, %, //, \*\*), Assignment (=, \+=), Comparison (==, \!=, \>), Logical (and, or, not).  
  * **Precedence:** A simplified hierarchy (Parentheses \> Exponentiation \> Multiply/Divide \> Add/Subtract \> Comparison \> Logical).  
* **Input & Output:**  
  * input(): To get data from the keyboard.  
  * print(): To display data on the screen.  
* **Control Structures:**  
  * **Selection:** if, elif, else.  
  * **Repetition:**  
    * for loop: for item in sequence:  
    * while loop: while condition:  
  * **Loop Control:** break (exit loop immediately) & continue (skip to the next iteration).

### **Part 4: The "Advanced" Phase \- Python Data Structures & Applications**

*This section covers how to structure larger programs and handle complex data in Python.*

* **Sub-programs (Functions):**  
  * def function\_name(parameter):  
  * return statement to send a value back.  
  * **Scope:** Global vs. Local variables.  
* **Core Data Structures (with key characteristics & methods):**  
  * String: Immutable sequence of characters.  
  * List: Ordered, **changeable** collection (\[\]). *Key methods: .append(), .insert(), .remove(), .sort(), .reverse(), del list\[i\].*  
  * Tuple: Ordered, **unchangeable** collection (()).  
  * Dictionary: Unordered, changeable collection of key:value pairs ({}). *Key methods: .keys(), .values(), .items(), .pop().*  
* **File Handling:**  
  * open() function with modes: "r" (Read), "a" (Append), "w" (Write), "x" (Create).  
  * Key functions: .read(), .readline(), .write(), .close().  
  * os module for file/directory deletion (os.remove(), os.rmdir()).  
* **Database Connectivity:**  
  * A brief note: Python uses a "connector" (e.g., mysql-connector) to import, create a cursor, execute SQL, and commit changes.  
* **Basic Algorithms in Python:**  
  * **Searching:** Sequential Search (linear scan).  
  * **Sorting:** Bubble Sort (comparing and swapping adjacent elements).  
    * Includes the concept of swapping variables (e.g., a, b \= b, a).