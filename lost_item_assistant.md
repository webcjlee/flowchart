```mermaid
flowchart TD
    A[Start: Student reports lost item] --> B{Ask detailed questions}
    B --> C[Collect item details (type, color, last seen, etc.)]
    C --> D[Suggest possible locations]
    D --> E[Student checks location]
    E --> F{Was item found?}
    F -- Yes --> G[End: Item found, process complete]
    F -- No --> H[Track attempt and location tried]
    H --> I{Have all locations been tried?}
    I -- No --> D
    I -- Yes --> J{Exceeded attempt limit?}
    J -- No --> D
    J -- Yes --> K[Notify: Item not found after multiple tries]
    K --> L[Provide next steps (report to lost & found, etc.)]
    L --> M[End: Process complete]
