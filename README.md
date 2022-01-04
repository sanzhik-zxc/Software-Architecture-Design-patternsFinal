# derivative-calculator





Calculates the symbolic derivative of the given function. It parses the expression first using recursive descent parsing
and then recusrsively calculates the derivative. It uses `MathJax` to render mathematical expressions written in `AsciiMath`

The following functions and operators are currently supported
functions: `ln`, `sqrt`, `sin`, `cos`, `tan`, `cot`, `sec`, `cosec`. operator: `unary and binary - and +`, `^ (exponential)`, 
`* (multiplication)`, `\ (division)` 

All arguments to functions should be enclosed in parentheses. for example : `sin(x+1), sqrt(x^2)`

## Operator Precedance
0. `ln`, `sqrt`, `sin`, `cos`, `tan`, `cot`, `sec`, `cosec`
1. `^`
2. `unary - and +`
3. `* and /`
4. `d/dx`
5. `binary - and +`

So, `d/dx a*b` means  `d/dx (a*b)`, but `d/dx a + b` means `(d/dx a) + b`. also `sin(x)^3` means `((sin(x))^3` and not `sin(x^3)`.


## Operator Associativity
1. left associative: `+`, `-`, `*`, `/`
2. right associative: `^`

So, `a*b/c/d` means `((a*b)/c)/d`, and `a^b^c` means `a^(b^c)`.

In case of power of trigonometric functions, you should provide input like `(sin(x))^3`, `sin^3(x)` will not work.




# screens


![first](https://user-images.githubusercontent.com/94376325/148031608-0ba772e5-1c4d-4518-b7c8-f080546e8b78.png)


![second](https://user-images.githubusercontent.com/94376325/148031471-947fff9e-a573-4bfb-ba86-72a7900c5145.png)

![third](https://user-images.githubusercontent.com/94376325/148031479-3947abcf-a6e1-4db0-b9aa-53f044770310.png)
