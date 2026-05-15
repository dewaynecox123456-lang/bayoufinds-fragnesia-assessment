# Operator Acknowledgment Model

This tool requires intentional execution by the operator.

Before running, the operator must:
1. Extract the package.
2. Grant execute permission to the script.
3. Manually launch the assessment.
4. Accept the on-screen disclaimer by typing `I ACCEPT`.

Automation may use:

```bash
--accept-disclaimer
```

This does not remove operator responsibility. It only allows scripted execution where the operator has already accepted the product terms.
