# Ruby Instance Variable Modification Bug

This repository demonstrates a common error in Ruby related to how instance variables are accessed and modified.  When you attempt to modify the value of an instance variable using its getter method, it won't actually change the internal state.  This is because the getter method only returns a copy of the variable's value, not a reference to the variable itself.

The `bug.rb` file shows the problematic code. The `bugSolution.rb` file offers a corrected approach.

## How to Reproduce

1. Clone this repository.
2. Run `ruby bug.rb`