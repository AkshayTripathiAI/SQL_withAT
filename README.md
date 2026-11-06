# SQL_withAT

Personal SQL practice notes: a single MySQL script covering the basics of creating databases and tables and inserting and selecting data.

## What's covered

[`learning_SQL.sql`](learning_SQL.sql) walks through:

- Creating, selecting and dropping databases (`CREATE DATABASE`, `IF NOT EXISTS`, `USE`, `DROP DATABASE`, `SHOW DATABASES`, `SHOW TABLES`)
- Creating and dropping tables with `PRIMARY KEY` and `NOT NULL` constraints
- Single-row and multi-row `INSERT` statements, with and without a column list
- `SELECT * FROM ...` to view table contents
- A practice exercise: a `COMPANY` database with an `EMPLOYEES` table
- A `college.student` table with roll number, name, marks, grade and city

## Running it

The script uses MySQL syntax (`USE`, `SHOW DATABASES`, double-quoted string literals). Run it in a MySQL client such as MySQL Workbench, or statement by statement from the CLI:

```bash
mysql -u <user> -p < learning_SQL.sql
```

Note that the script is a sequence of practice steps: it drops and recreates databases and tables (`college`, `COMPANY`, `student`) along the way, so run it against a scratch MySQL instance, not one with data you want to keep.
