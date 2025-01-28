# Unreachable `println` Statement in Julia

This example demonstrates an uncommon error in Julia: an unreachable `println` statement.  While not strictly a bug, it can lead to confusion if one expects the output to be shown.

The code defines a function `myfunction` that squares its input, negating it if it's negative. However, the `println` statement within the function is never executed because the function always returns before reaching it.  The compiler will optimize this line away.

The solution involves removing the unreachable `println` statement, making the code cleaner and more efficient.