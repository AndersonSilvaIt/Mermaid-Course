::: mermaid
    stateDiagram-v2

    state fork <<fork>>

    [*] --> state1
    state1 --> fork
    fork --> state2    
    fork --> state3

    state join1 <<join>>
    state2 --> join1
    state3  --> join1

    join1 --> state4

    state4 --> [*]

    direction LR