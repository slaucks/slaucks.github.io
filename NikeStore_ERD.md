```mermaid
erDiagram
    CUSTOMER ||--o{ ORDER : places
    CUSTOMER {
           String Name
           string deliveryaddress
           string itemnumber
}
    ORDER||--|{ LINE-ITEM : contains
    ORDER { 
       string OrderNumber
       string customernumber
       string itemnumber
}
    SALE ||--o{ ORDER : contains
    SALE { 
       string OrderNumber
       string customernumber
       string itemnumber
       string saleprice
    }
    INVENTORY }||--o{ LINE-ITEM : contains
    LINE-ITEM {
          string productcode
          int quantity
          float priceperunit
    }

```