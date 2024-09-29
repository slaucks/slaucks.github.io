```mermaid
erDiagram
    CUSTOMER ||--o{ ORDER : places
    CUSTOMER {
           String Name
           String Customer Number
}
    SALE ||--|{ LINE-ITEM : contains
    SALE { 
       int OrderNumber
       string delivery address
}
    CUSTOMER }|..|{ DELIVERY-ADDRESS : uses
    LINE-ITEM {
          string productcode
          int quantity
          float priceperunit
}

```