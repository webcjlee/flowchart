Count 1 to 10
```mermaid
flowchart TD
    Start([Start]) --> Init[Set i = 1]
    Init --> Check{Is i <= 10?}
    Check -- Yes --> Count[Print i]
    Count --> Inc[Increment i by 1]
    Inc --> Check
    Check -- No --> End([End])
