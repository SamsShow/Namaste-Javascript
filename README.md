# NAMASTE 🙏🏻 JAVASCRIPT

Everything in JavaScript happens inside an **EXECUTION CONTEXT**. It is like a big box with two components:

1. **Memory Component**
   - All variables and functions are stored as key-value pairs.
   - This memory component is also known as the variables environment.

2. **Code Component**
   - Code is executed one line at a time.
   - Also known as the Thread of Execution.

JavaScript is a **SYNCHRONOUS SINGLE-THREADED** language, meaning it can execute one command at a time in a specific order.

## Execution Context Phases:

1. **Memory Creation Phase**
   - Allocates memory to all variables and functions.
   - Memory is allocated as `undefined` to the variables.

2. **Code Execution Phase**
   - Runs line by line.
   - Values are allocated to the variables.
   - When a function is invoked, a new execution context is created.
   - When a value is returned in a function, the entire execution context gets deleted.

JavaScript has its own **CALL STACK** to manage these execution contexts. It's a stack, and the global execution context is at the bottom of this stack. When a function is executed, its execution context is placed above in the stack, maintaining the order of execution.

**HOISTING** in JavaScript allows accessing functions and variables even before initializing them.

JavaScript has its own **CALL STACK** to manage the execution context order. It can be referred to as a Program Stack, Runtime Stack, Control Stack, or Machine Stack.

**Undefined** is a special keyword in JavaScript with the following meanings:

- It is assigned to variables during the memory creation phase.
- It means a variable has been declared but not defined.

**Not Defined** refers to trying to access a variable that is not declared in the code, resulting in an error.

JavaScript is a loosely typed or weakly typed language, meaning it does not attach variables to specific data types. Variables can hold any type of data.

Never manually assign `undefined` to a variable.

**Note:** The global object is created (window), and the `this` keyword is created. Both point to the same place in the global space.

**Note:** An empty JavaScript program is the shortest JavaScript program. The JavaScript engine works even in an empty program, creating a global object, a global execution context, and setting up `this`.

If we have the same variable names in different execution contexts, JavaScript will execute the code line by line, creating separate execution contexts for functions, leading to separate values for the same variable.

Empty JavaScript programs still involve the creation of a global object (window), a global execution context, and the `this` keyword.
