:::mermaid
sequenceDiagram

    participant User as "User"
    participant App as "Messaging App"
    participant Server as "Message Server"

    User->>App: Open Messaging App
    activate App

    loop Check for new Messages
        App->>Server: Request New Messages
        activate Server
        Server-->>App: New Message(s)
        deactivate Server
    end

    App-->>User: Display Messages
    deactivate App
