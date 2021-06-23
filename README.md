# postgres-pgdump
https://www.eksworkshop.com/intermediate/201_resource_management/advanced-pod-limits/


kubectl exec -i postgres-0 -- pg_dumpall -c -U postgres > postgres_sql_dump.sql
cat postgres_sql_dump.sql | kubectl exec -i postgres-0 -- psql -U postgres

CRONJOB
