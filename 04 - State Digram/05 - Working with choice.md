:::mermaid
stateDiagram-v2
    state userAcctount <<choice>>

    [*] --> CheckBalance
    CheckBalance --> userAcctount
    userAcctount --> InsufficienteFunds: if balance < amount

    userAcctount --> WithdrawlSuccess: if balance>= amont

    InsufficienteFunds --> [*]
    WithdrawlSuccess --> [*]

    state InsufficienteFunds {
        [*] --> NotifyUser
        NotifyUser --> [*]
    }

    state WithdrawlSuccess {
        [*] --> DispenseCash
        DispenseCash --> [*]
    }