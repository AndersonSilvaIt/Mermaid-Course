::: mermaid

---
title: Car Design States
---

stateDiagram-v2
    direction LR
    [*] --> Design
    Design --> Produce
    Produce --> Assembly
    Assembly --> Test
    Test --> Deliver
    Deliver --> [*]
