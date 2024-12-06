:::mermaid

stateDiagram-v2

    classDef notMoving fill: white, color:black
    classDef movement font-style: italic
    classDef badBadEvent fill:#f00,color:white,front-weight:bold,stroke-width:2px,stoke:yellow
    classDef run fill:green, color:white

    [*]--> Still
    Still --> [*]
    Still --> Moving
    Moving --> Still
    Moving --> Running ::: run
    Running --> Crash
    Crash --> [*]

    class Still notMoving
    class Moving movement
    class Running run
    %%class Crash badBadEvent

    direction LR