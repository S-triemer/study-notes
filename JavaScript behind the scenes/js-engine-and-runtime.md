# What is the JS Engine

A Program that executes JS code.  
Every Browser has it's own engine (most famous: v8, powers google chrome and node js)

Every engine contains a call stack and a heap

- Call Stack: Where the code is executed
- Heap: unstructured memory pool that stores all the objects in memory that the application needs.

## compilation vs. interpretation

compilation: entire code is converted into machine code at once, and written to an binary file that can be executed on a computer. The execution can happen way after the compilation.
interpretation: interpreter runs through the source code and executes it line by line.  
just in time compilation: entire code is converted into machine code at once and then gets executed immediately.

## javascripts just in time compilation

1. When code enters the engine it gets parsed (read) into a data structure called AST (abstract syntax tree).
2. compilation: takes the AST and compiles an unoptimized version of machine code.
3. Executes the compiled code immediately
4. optimization (during execution): optimizes the unoptimized version of machine code and compiles it again without stoping execution.

# What is a Javascript runtime

Includes all the things that are needed to use javascript (in the browser).

- JS Engine
- Web APIs (DOM, Timers, Fetch API...) provided from the engine but not part of javascript itself; accessible via the global window object.
- Callback Queue: Data structure that contains all the callbackfunctions that are ready to be executed.
  e.g. eventlistener function: when the event happens, the callback function is put into the callback queue. When the callstack is empty, the function is passed to the call stack by the event loop.
