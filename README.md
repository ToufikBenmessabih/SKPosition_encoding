# SKPosition_encoding
Position Encoding Using Trigonometric Functions.

### Formula

The position encoding can be described by the following formula:

`p_n(x) = (sin(2^0 π x), cos(2^0 π x), sin(2^1 π x), cos(2^1 π x), ..., sin(2^N π x), cos(2^N π x))`

Where:

- `x` represents the position or time step.
- `N` is the highest exponent in the series, determining the number of terms.
- `π` is the mathematical constant Pi (approximately 3.14159).

### Explanation
The formula generates a sequence of sine and cosine values at different frequencies. The terms are generated as follows:

For each integer i from 0 to N:
- Compute `sin(2^i π x)`
- Compute `cos(2^i π x)`
- Concatenate these values into a single list.

This encoding allows the model to learn positional dependencies.
