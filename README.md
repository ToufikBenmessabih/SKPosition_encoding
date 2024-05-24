# Position_encoding
Position Encoding Using Trigonometric Functions.
Notebook: `SKpose_spacial_position_encoding.ipynb`

### Formula

The position encoding can be described by the following formula:

$`p_n(x) = (\sin(2^0 \pi x), \cos(2^0 \pi x), \sin(2^1 \pi x), \cos(2^1 \pi x), \ldots, \sin(2^N \pi x), \cos(2^N \pi x))`$


Where:

- $`x`$ represents the position coordinates (x,y,z) separatly.
- $`N`$ is the highest exponent in the series, determining the number of terms.
- $`\pi`$ is the mathematical constant Pi (approximately 3.14159).

### Explanation
The formula generates a sequence of sine and cosine values at different frequencies. The terms are generated as follows:

For each integer i from 0 to N:
- Compute $`\sin(2^i \pi x)`$
- Compute $`\cos(2^i \pi x)`$
- Concatenate these values into a single list.

This encoding allows the model to learn positional dependencies.

# Concatenate the position_encoding with the input
Notebook: `concat (pe, X).ipynb`


