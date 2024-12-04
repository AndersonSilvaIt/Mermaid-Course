:::mermaid

sequenceDiagram
    Alice->>Bob: Hello Bob, how are you?
    alt is sick?
        Bob->>Alice: Not so good
    else Not sick
        Bob->>Alice: Feeling like a Daisy
    end

    opt Other response
        Bob->>Alice: Thanks for Asking
    end