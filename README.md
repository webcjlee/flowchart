flowchart TD
   A[Start Game] --> B[Display Question]
   B --> C[Get User Answer]
   C --> D{Is Answer Correct?}
   D -- Yes --> E[Update Score]
   D -- No --> F[Show Correct Answer]
   E --> G{More Questions?}
   F --> G
   G -- Yes --> B
   G -- No --> H[End Game]
