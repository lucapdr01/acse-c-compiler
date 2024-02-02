## ACSE (Advanced Compiler System for Education) Overview

ACSE serves as a comprehensive toolchain designed for educational purposes within the domain of "Formal Languages and Compilers." It provides students with a simplified yet insightful exploration of the compilation and execution processes of computer programs. The toolchain comprises three integral components:

- **ACSE compiler**: Translates programs written in the LANCE language, a simplified C-like language, into assembly language code compatible with the fictional MACE architecture.
- **Assembler**: Converts assembly code into binary executable object files.
- **MACE simulator**: Facilitates program execution by interpreting these object files.

ACSE aims to demystify the complexities of compiler construction and execution, offering students a hands-on understanding of the fundamental principles underlying computing systems.

## ACSE Feature Addition: Iterated Expressions

Welcome to the latest enhancement to ACSE, introducing Iterated Expressions to the LANCE language. This feature extends the capabilities of the compiler toolchain, enabling the evaluation of iterative computations through the `repeat_exp` statement.

### Feature Overview

The `repeat_exp` statement allows for the implementation of simple loops within LANCE programs, facilitating repetitive computation by re-evaluating an expression and assigning it to a variable for a specified number of iterations.

### Syntax

```plaintext
repeat_exp(<var.> = <exp.1>, <exp.2>, <exp.3>);
```

### Behavior

- Iterates `<exp.2>` times, re-computing `<exp.3>` and assigning it to `<var.>` at each iteration.
- If `<exp.2>` is zero or negative, the loop does not iterate, leaving `<var.>` with its initial value (`<exp.1>`).

### Example Usage

```c
repeat_exp(a = 0, 10, a + 1);
```

### Advanced Usage

Explore more complex computations, such as implementing recurrent formulas.

Thank you for choosing ACSE for your educational journey in compilers and formal languages. I hope this new feature enriches your learning experience.
