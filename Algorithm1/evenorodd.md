## 1. Check Even or Odd Number

Design an algorithm and flowchart that take a number as input and
determine whether it is even or odd.

### ✔ Pseudocode

```text
START

    INPUT number

    IF number % 2 == 0 THEN

        PRINT Even

    ELSE

        PRINT Odd

    ENDIF

END
```

### ✔ Flowchart

```mermaid
  flowchart TD
    start(["Start"]) --> input[/"Input number n"/]
    input --> check{"Is n mod 2 = 0?"}
    check -->|Yes| even["Output: Even"]
    check -->|No| odd["Output: Odd"]
    even --> finish(["End"])
    odd --> finish

    classDef terminal fill:#eef2ff,stroke:#818cf8,color:#1e1b4b
    classDef inputOutput fill:#ecfeff,stroke:#22d3ee,color:#083344
    classDef decision fill:#fefce8,stroke:#facc15,color:#422006
    classDef evenResult fill:#f0fdf4,stroke:#4ade80,color:#052e16
    classDef oddResult fill:#fff7ed,stroke:#fb923c,color:#431407

    class start,finish terminal
    class input inputOutput
    class check decision
    class even evenResult
    class odd oddResult


