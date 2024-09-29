```mermaid
erDiagram
    CUSTOMER ||--o{ ORDER : places
    CUSTOMER {
           String Name
           Item Itemnumber
           String Ordernumber
           string deliveryaddress
}
    SALE ||--|{ ORDER : contains
    SALE { 
       OrderNumber
       customernumber
    }
    CUSTOMER }|..|{ LINE-ITEM : contains
    LINE-ITEM {
          string productcode
          int quantity
          float priceperunit
    }

```