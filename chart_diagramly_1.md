
```mermaid
flowchart TD
    Start[Start Game] --> DisplayQ[Display Question]
    DisplayQ --> GetAns[Get User Answer]
    GetAns --> IsCorrect{Is Answer Correct?}
    IsCorrect -->|Yes| UpdateScore[Update Score]
    IsCorrect -->|No| ShowAnswer[Show Correct Answer]
    UpdateScore --> MoreQ{More Questions?}
    ShowAnswer --> MoreQ
    MoreQ -->|No| EndGame[End Game]
    MoreQ -->|Yes| DisplayQ
