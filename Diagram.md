```mermaid

stateDiagram-v2
    s1 : Becomes solid
    s2: Turns to steam
    
    Water --> Freezes
    Water --> Boils

    Freezes --> s1
    s1 --> Grows
    Boils --> s2
    s2 --> Evaporates 
```