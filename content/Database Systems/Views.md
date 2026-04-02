```sql
CREATE VIEW v_invoice
AS 
SELECT InvoiceId, CustomerId, InvoiceData, BillingCountry FROM Invoice WHERE InvoiceId = 2

SELECT * FROM v_invoice
```

(Basically a virtual table)