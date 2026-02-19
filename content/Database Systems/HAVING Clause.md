incorrect: 
```sql
SELECT count (*), firstname from Employee
group by firstname
having count(*) > 1
```

