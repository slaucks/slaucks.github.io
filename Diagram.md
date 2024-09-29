```mermaid

stateDiagram-v2
    If --> Up
    Up --> Down

    Down --> Further
    Up --> Away
    Away --> Fly
    Further --> [*]
    Fly --> [*]
```