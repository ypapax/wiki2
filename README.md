# Postgres Query which gives you answer to question: what queries uses most db writes:
select * from pg_stat_statements order by wal_records desc;
