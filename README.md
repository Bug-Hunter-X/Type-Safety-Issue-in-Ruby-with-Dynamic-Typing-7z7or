# Ruby Type Safety Example

This repository demonstrates a potential type safety issue that can arise in Ruby due to its dynamic typing system. The code showcases a class with a setter and getter for a variable, which accepts different types without explicit type checking.  This could lead to runtime errors or unexpected results if not carefully managed in larger applications.

The `bug.rb` file contains the example code that exhibits the issue. The `bugSolution.rb` file suggests a way to mitigate the problem (although perfect type safety isn't possible in Ruby without external tools).

## Running the Code

1. Clone the repository.
2. Navigate to the repository directory.
3. Run `ruby bug.rb` and `ruby bugSolution.rb` to see the outputs.

## Solutions and Mitigation

While Ruby's dynamic typing is powerful, it's essential to be mindful of potential type-related issues.  Consider these approaches:

* **Stronger Encapsulation:** Use private instance variables and more restrictive public methods to enforce stricter type usage (see `bugSolution.rb` for a basic example of this).
* **Runtime Checks:** Add explicit checks within the setter method to validate the type of the input.
* **Static Analysis Tools:** Tools like RuboCop can help identify potential type-related issues by detecting inconsistencies in your code.
* **Consider Type-Safe Libraries:** Use libraries that offer more robust type handling or use a more strictly-typed language if type safety is critical to your project.

This example serves as a reminder to be aware of the tradeoffs of dynamic typing and to write defensive code to prevent unexpected behavior.