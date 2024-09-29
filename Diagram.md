```mermaid

stateDiagram-v2
    s1 : Becomes solid
    s2: Turns to steam
    s3: Becomes rain

    Water --> Freezes
    Water --> Boils

    Freezes --> s1
    s1 --> Grows
    Boils --> s2
    s2 --> Evaporates 
    Evaporates --> s3
    s3 --> Water
    Grows --> Thaws
    Thaws --> Water
```