::: mermaid

graph
    subgraph one[single]

        A1

    end

    subgraph two[double]
        B1 --> B2
    end

    subgraph three[triple]
        C1 --> C2 & C3
    end        

    one --> two --> three