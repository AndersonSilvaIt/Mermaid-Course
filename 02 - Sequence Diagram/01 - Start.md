::: mermaid

sequenceDiagram
    Actor Manager
    participant Alice as sup1
    participant James as sup2
    participant Bob as sub3

    Manager->>Alice: Call a meeting, now
    Alice->>James: Hi James, It's Alice
    James->>Alice: Hello Alice
    Alice->>Bob: Are you there Bob