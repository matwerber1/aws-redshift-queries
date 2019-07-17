# aws-redshift-queries

A catalog of Redshift / Postgres queries that I use


# Stored Procedures

## List stored procedures

```sql
SELECT  proname 
FROM    pg_catalog.pg_namespace n 
JOIN    pg_catalog.pg_proc p 
ON      pronamespace = n.oid 
WHERE   nspname = 'public';
```