```mermaid
erDiagram
    CUSTOMER ||--o{ ORDER : places
    CUSTOMER {
           String Name
           String Ordernumber
           string deliveryaddress
}
    SALE ||--|{ LINE-ITEM : contains
    SALE { 
       int OrderNumber
       string customer number
    }
    CUSTOMER }|..|{ DELIVERY-ADDRESS : uses
    LINE-ITEM {
          string productcode
          int quantity
          float priceperunit
    }

```