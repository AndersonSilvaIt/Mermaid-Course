::: mermaid

stateDiagram-v2
    %%state "Card Design" as Design
    Design: Card Design
    %%direction LR
    [*] --> Design
    Design --> Produce : activate design
    Produce --> [*]
