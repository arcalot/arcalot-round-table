# Expansion of Workflow Expression Language

## Background

The current state of the expression language allows users to retrieve values from inputs and step output. That is enough for usable workloads, but is insuffient for many use cases.

Examples of situations which are limited right now:
- Can't import values from files (will be done with a function)
- Can't conditionally run sections (will be done with a conditional expression and a sub-workflow)
- Can't do comparisons or math with known values for inputs and outputs. (Will be done with conditional expressions and mathematical expressions)

This proposal will make it so less manual work is required to get a workflow working.

## Proposal

Proposed changes:
- Make subexpressions default within map access since it is unintuitive as-is, removing the old () syntax. Moving from `map[(sub-expression)]` to `map[sub-expression]`
- Add functions. Would be added as a root item, and therefore would work where subexpressions are supported. That would also make it so an expression can be exclusively a function call. The functions will be strongly typed, with a standardized interface for their inputs and outputs, allowing type verification.
- Add binary comparison operators. This would need to be another root item. This would be simple. `expression ==|!=|<|>|<=|>= expression`. Types must match, or else there will be a type error.
- Mathematical expressions. These would be simple binary mathematical operators, with the potential for parentheses for ordering changes. Will be strongly typed.

Detailed issues for proposed changes:
- [Functions](https://github.com/arcalot/arcaflow-expressions/issues/1)
- [Binary Comparison Operators](https://github.com/arcalot/arcaflow-expressions/issues/2)
- [Mathematical Expressions](https://github.com/arcalot/arcaflow-expressions/issues/3)

### Priorities 
- The function calls and comparison operators will be the top priorities
- Mathematical expressions will be lower priority, with most of the work based on the work for the comparison operators.

### Approval
By approving this proposal, you agree to the addition of functions, binary comparison operators, and mathematical expressions to the language. Not necessarily the way it's implemented.

Discussion on how it is implemented can be debated in the issues in the expression repository linked above.

## Drawbacks
- It adds complexity to the language
