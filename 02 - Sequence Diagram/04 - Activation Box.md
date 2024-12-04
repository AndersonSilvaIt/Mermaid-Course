:::mermaid

sequenceDiagram

    Server->>Database: Give me data
    activate Database
    Database-->>Server: here you go
    deactivate Database
