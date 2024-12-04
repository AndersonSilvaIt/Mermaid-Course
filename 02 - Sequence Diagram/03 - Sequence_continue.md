:::mermaid

sequenceDiagram
    Alice ->> Bob: Hello, how are you?
    Bob->>Alice: Fine, thank you And you?
    create participant Carl
    Alice->>Carl: Hi Carl, What up?
    Carl--)Alice: I am fine Alice
    create actor D as Donald
    Carl-->D: Hi!
    destroy Carl
    Alice-xCarl: Bye bye Carl
    D--)Bob: great job Bob
    destroy Bob
    Bob --xAlice: Have a nice Day