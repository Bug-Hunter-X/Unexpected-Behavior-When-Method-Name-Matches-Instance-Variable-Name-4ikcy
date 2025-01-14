# Ruby Bug: Unexpected Instance Variable Behavior
This repository demonstrates a subtle bug in Ruby where a method with the same name as an instance variable overshadows the instance variable's assignment. The bug arises from the precedence given to the method definition over the instance variable.  This leads to unexpected behavior when attempting to modify the instance variable through the method.

## How to Reproduce
1. Clone the repository.
2. Run `ruby bug.rb`.
3. Observe that the value of the instance variable `@value` remains unchanged despite the attempted assignment.

## Solution
The solution involves either renaming the method or using a different approach to access/modify the instance variable.

## Lessons Learned
This bug highlights the importance of careful naming conventions to avoid conflicts between methods and instance variables in Ruby.  A clear naming strategy can prevent unexpected behavior and improve code maintainability.