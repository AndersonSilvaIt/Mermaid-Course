:::mermaid

sequenceDiagram
    actor User as  "End User"
    participant App as "Application"
    participant Server as "Server"
    participant DB as "Database"

    User->>App: Request Data
    activate App
    
    App->> Server: Fetch Data
    activate Server
    alt Data Exists?
        Server->> DB: Query Database
        activate DB

        DB--)Server: Return Data
        deactivate DB
        Server--)App: Return Data
    else Data Not exists
        Server--xApp: Terminate ( Data not Found )
    end

    deactivate Server
    App --) User: Display Data
deactivate App




    