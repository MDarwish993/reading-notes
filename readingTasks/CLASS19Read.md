# Class 19

### 1. Can you change the state of a data structure using functional programming?
  In purely functional programming, data structures remain immutable. You cannot directly alter their state once created. Instead, operations on data structures generate new ones with the desired modifications, preserving the original structure. This emphasis on immutability ensures referential transparency and prevents problems associated with mutable state.

### 2. Define purely functional programming.
   Purely functional programming is a paradigm where all computation is treated as the evaluation of mathematical functions. It relies on pure functions that:
- Always produce the same output for the same input, independent of hidden or external state.
- Avoid side effects, such as modifying external state or performing non-computational actions.
- Steer clear of mutable data structures, creating new ones for changes.

The central concept is referential transparency, ensuring a function's result depends solely on its inputs, with no hidden state changes. This approach simplifies code reasoning, encourages modularity, and facilitates parallelization and optimization.

### 3. How do you think purely functional programming will differ from the programs you’ve written so far in this course?
   If you have been writing programs in an imperative or object-oriented style in your course, transitioning to purely functional programming will involve some fundamental differences:

   a. Immutability: In purely functional programming, you will need to adopt immutability as a core principle. Instead of modifying variables or data structures in-place, you'll create new ones with the desired changes. This can lead to a different way of thinking about data manipulation.

   b. No Side Effects: Purely functional programs avoid side effects, such as I/O operations or modifying global state. This means you'll need to embrace techniques like monads or purely functional I/O libraries to perform I/O operations.

   c. Functional Composition: You'll rely heavily on functional composition, using higher-order functions to build complex functionality by combining smaller, pure functions. This can lead to more concise and modular code.

   d. Recursion: Functional programming often leans on recursion instead of loops for iteration. You'll need to become comfortable with recursive algorithms and understand tail recursion for efficient function calls.

   e. Parallelism and Concurrency: Purely functional programs are well-suited for parallelism due to their lack of shared mutable state. You may explore parallel and concurrent programming techniques that are different from traditional approaches.
