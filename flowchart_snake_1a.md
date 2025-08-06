# Snake Game Flowchart

```mermaid
flowchart TD
    A([Start Game]) --> B([Initialize Snake, Food, Score, and Game Window])
    B --> C([Display Snake and Food])
    C --> D([Read User Input,Direction])
    D --> E([Update Snake Position])
    E --> F{Did Snake Hit Wall or Itself?}
    F -- Yes --> G([Game Over])
    F -- No --> H{Did Snake Eat Food?}
    H -- Yes --> I([Increase Score and Snake Length])
    I --> J([Generate New Food])
    J --> C
    H -- No --> C
    G --> K([Display Final Score])
    K --> L{Play Again?}
    L -- Yes --> B
    L -- No --> M([End Game])
