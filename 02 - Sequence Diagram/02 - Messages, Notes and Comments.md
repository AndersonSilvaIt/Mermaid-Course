::: mermaid

sequenceDiagram
    Actor Manager
    Note over Alice, James: text here <br/> Now

    Manager->>Alice: Call a meeting, now
    Alice->>James: Hi James, It's Alice
    James->>Alice: Hello Alice
    Alice->>Bob: Are you there Bob

    % Note comment
    % Note <positivon> of <object(s)>: <description>

    % message Symbols
    % - Solid Line
    % -- Dotted Line
    % > No Arrow
    % >> Filled Arrow (sync)
    % ) stick arrow ( async )
    % X 