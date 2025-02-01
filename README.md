# Uninitialized Integer Variable in Go

This example demonstrates a common issue in Go where an integer variable is used before it's explicitly initialized.  While Go initializes variables to their zero value, this behavior might not always be obvious or intended, especially when dealing with increment/decrement operations.

**The Bug:**
The `main` function declares an integer variable `i` but doesn't assign it an initial value.  Go will initialize it to 0, but the output may not be what's intuitively expected when incrementing it.

**The Solution:**
Explicitly initialize the variable `i` to a specific value before using it. This clarifies the intention and makes the code more robust and predictable.