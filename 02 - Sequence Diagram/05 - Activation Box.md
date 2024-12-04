:::mermaid

sequenceDiagram
    participant User
    participant App as "Shopping App"
    participant Gateway as "Payment Gateway"
    participant Bank

    User->>App: Select Item and Checkout
    activate App
    App->>Gateway: Initiate Payment Request
    activate Gateway
    Gateway->>Bank: Process Payment
    activate Bank
    Bank-->>Gateway: Payment Approved
    deactivate Bank
    Gateway-->>App: Payment Success
    deactivate Gateway

    App-->>User: Order Confirmed
    deactivate App
