```mermaid
flowchart TD
 Start([Start]) --> id1([Guess a number 1 through 10]) --> id2([Player enters their number])
id2 --> ([High]) 
id2 --> ([Low])
id2 --> ([Correct!]) --> End([End])
```