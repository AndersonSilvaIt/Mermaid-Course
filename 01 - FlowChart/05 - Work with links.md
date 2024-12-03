::: mermaid 

flowchart
    A([start]) --> B[/Input x/]
    B --> C{x > 5 ?}
    C -..-> |yes|D((stop))
    C --> |no|F[/print x/]
    F --> G[x = x + 1]
    G --> C
