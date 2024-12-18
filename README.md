# Ruby Bug: Unexpected Setter Behavior

This repository demonstrates a subtle bug in Ruby related to the unexpected side effects of using `puts` within a setter method.  The bug causes unexpected output and potentially alters the program's intended behavior.

## Bug Description
The `MyClass` class defines a setter method (`value=`) that prints a message to the console using `puts`. This seemingly innocuous addition leads to unexpected behavior when the setter is called within a larger program flow.

## How to Reproduce
1. Clone this repository.
2. Run `bug.rb`.
3. Observe the unexpected output caused by the `puts` statement in the setter method.

## Solution
The solution involves refactoring the setter method to avoid the `puts` statement, either by removing it entirely or by using a different approach for logging or debugging if such output is needed.