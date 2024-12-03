
<!-- 
    TB - Top to bottom
    TD - Top-down / same as top to bottom
    BT - Bottom to top
    RL - Right to left
    LR - Left to right
 -->

::: mermaid
flowchart TB
    A[start]; B[car]; C[toy]
    
    A --> B
    A --> C & D
    C --> F
    B --> F
    D --> G
    D --> g
    