# From Two-Digit Multiplication to Convolution

This project contains an expository mathematics paper by Albert Stockton about the connection between:

- positional number systems,
- polynomial multiplication,
- discrete convolution,
- carrying in an arbitrary base, and
- fast integer multiplication algorithms.

The paper begins with the two-digit identity

```text
(10a + b)(10c + d) = 100ac + 10(ad + bc) + bd
```

and generalizes it to numbers written in any base `B`:

```text
(sum a_i B^i)(sum c_j B^j)
    = sum_k (sum_{i+j=k} a_i c_j) B^k.
```

The inner sum is the discrete convolution of the digit sequences. Carrying then normalizes the coefficients into valid base-`B` digits.

## Paper

The complete LaTeX source is in [`main.tex`](main.tex).

## Compile

Using a local LaTeX installation:

```bash
pdflatex main.tex
pdflatex main.tex
```

Or upload `main.tex` to Overleaf and compile it with pdfLaTeX.

## Central conclusion

> Place-value arithmetic is polynomial arithmetic evaluated at the base, followed by carrying.

## Note on originality

The mathematical ideas discussed here are established. The paper presents Albert Stockton's independent route to the result and develops it as an educational explanation rather than claiming a new theorem.
