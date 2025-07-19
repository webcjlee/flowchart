
               Title of File here
```mermaid
%% chart2 file
flowchart TD
line6 --> A
    A[Start] --> B[Initialize n = 2]
    B --> C{Is n < 100?}
    C -- No --> G[End]
    C -- Yes --> D[Check if n is prime]
    D --> E{Is n prime?}
    E -- Yes --> F[Print n]
    E -- No --> H[Do nothing]
    F --> I[Increment n by 1]
    H --> I
    I --> C
