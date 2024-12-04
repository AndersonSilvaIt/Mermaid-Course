:::mermaid
sequenceDiagram
    critical Estabilish connection to DB
        Service-->DB: Connect

    option Network Timeout
        Service-->Service: Log error    
    option Credentials rejected
        Service-->Service: Log different error
    end
    
