<!-- 
    TB - Top to bottom
    TD - Top-down / same as top to bottom
    BT - Bottom to top
    RL - Right to left
    LR - Left to right
 -->

::: mermaid
flowchart TB
    A["A:Family()"]; B[Man]; C[Woman]
    
    A --> B
    A --> C & D[Children]
    C --> F
    B --> F
    D --> G
    D --> g
    