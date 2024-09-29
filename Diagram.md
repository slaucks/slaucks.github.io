```mermaid

stateDiagram-v2
    s1 : Becomes solid
    s2: Turns to steam
    s3: Becomes rain
    s4: Water
    Water --> Freezes
    Water --> Boils

    Freezes --> s1
    s1 --> Grows
    Boils --> s2
    s2 --> Evaporates 
    Evaporates --> s3
    s3 --> s4
    Grows --> Thaws
    Thaws --> s4
```