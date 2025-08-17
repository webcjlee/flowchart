```mermaid
flowchart TD
    A([Start]) --> B[Display Question (e.g., "What is 7 × 8?")]
    B --> C[Get Answer from user]
    C --> D{Check Answer \n(Correct or Incorrect?)}
    D --> E[Update Score]
    E --> F{More questions?}
    F -- Yes --> B
    F -- No --> G([End])
```
