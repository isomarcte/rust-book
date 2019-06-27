# Variables #

> There are multiple trade-offs to consider in addition to the prevention of bugs. For example, in cases where you’re using large data structures, mutating an instance in place may be faster than copying and returning newly allocated instances. With smaller data structures, creating new instances and writing in a more functional programming style may be easier to think through, so lower performance might be a worthwhile penalty for gaining that clarity.

This remark is generally true, and especially true when using the standard data structures for normal mutable code, however it becomes much less of a performance hit if different data structures which are conducive to functional data copying are used, such as a tree based map.

# Functions #

> In function signatures, you must declare the type of each parameter. This is a deliberate decision in Rust’s design: requiring type annotations in function definitions means the compiler almost never needs you to use them elsewhere in the code to figure out what you mean.

Haskell is still king for inference here, though you should never use Haskell that way.

## Statements Vs. Expresssion ##

In Haskell and in FP based Scala, function bodies are usually (always in Haskell) an expression.

# Control Flow #

> It’s also worth noting that the condition in this code must be a bool. If the condition isn’t a bool, we’ll get an error. For example, try running the following code:

This is for C programmers.

## Loops ##

Loops are particularly important in rust because of no TCO.
