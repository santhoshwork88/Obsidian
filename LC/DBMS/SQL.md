1. What is relational Database.
		A relation database is used to store in a table format that is rows and columns.
		which will help to get the data more efficiently. Each row can be identified with a unique key.
2. Benefits of RDMS.
		- Data is stored in structured format
		- Uses query Language to retrieve data efficiently.
		- Provides data integrity.
		- Every Transaction has ACID properties.
3. Sql vs NoSql databses.
4. Only MySQL has the column reordering option while adding column in a table.

```sql
Alter table table_name add (column name datatype()) First; --add the column to the first
Alter table table_name add (column name datatype()) after name; --add the column after name column
```
5. COMMENT is used to comment on a column or table, only MYSQL supports inline comment that is comment a table or a column while creating or altering.

## SQL Languages:

| Language                           | Commands                                                             |
| ---------------------------------- | -------------------------------------------------------------------- |
| DDL - Data Definition Language     | CREATE, DROP, ALTER, TRUNCATE, COMMENT, RENAME                       |
| DML - Data Manipulation Language   | INSERT, UPDATE, DELETE, LOCK, CALL, EXPLAIN PLAN(dbms_xplan.display) |
| DCL - Data Control Language        | GRANT, REVOKE                                                        |
| TCL - Transaction control Language | BEGIN TRANSACTION, COMMIT, ROLLBACK, SAVEPOINT                       |
| DQL - Data Query Language          | SELECT                                                               |

## 📘 1. String Data Types

| Purpose         | Oracle        | MySQL                      | PostgreSQL            |
| --------------- | ------------- | -------------------------- | --------------------- |
| Fixed length    | `CHAR(n)`     | `CHAR(n)` / `CHARACTER(n)` | `CHAR(n)`             |
| Variable length | `VARCHAR2(n)` | `VARCHAR(n)` / `TEXT`      | `VARCHAR(n)` / `TEXT` |
| Unbounded text  | `CLOB`        | `TEXT`, `LONGTEXT`         | `TEXT`                |

---

## 🔢 2. Numeric Data Types

| Purpose             | Oracle                  | MySQL                                  | PostgreSQL                      |
| ------------------- | ----------------------- | -------------------------------------- | ------------------------------- |
| Integer             | `NUMBER`, `INTEGER`     | `INT`, `TINYINT`, `SMALLINT`, `BIGINT` | `INTEGER`, `SMALLINT`, `BIGINT` |
| Decimal / Fixed     | `NUMBER(p,s)`           | `DECIMAL(p,s)`, `NUMERIC(p,s)`         | `NUMERIC(p,s)`, `DECIMAL(p,s)`  |
| Float / Approximate | `FLOAT`, `BINARY_FLOAT` | `FLOAT`, `DOUBLE`, `REAL`              | `REAL`, `DOUBLE PRECISION`      |

---

## 📅 3. Date and Time Data Types

| Purpose             | Oracle                      | MySQL                              | PostgreSQL                  |
|---------------------|-----------------------------|------------------------------------|-----------------------------|
| Date only           | `DATE`                      | `DATE`                             | `DATE`                      |
| Date + time         | `TIMESTAMP`                 | `DATETIME`, `TIMESTAMP`           | `TIMESTAMP`                 |
| Time only           | `INTERVAL DAY TO SECOND`    | `TIME`                             | `TIME`                      |
| Time zone support   | `TIMESTAMP WITH TIME ZONE`  | `TIMESTAMP` (server TZ)           | `TIMESTAMP WITH TIME ZONE` |

---

## 📦 4. LOB / Binary Data Types

| Purpose      | Oracle            | MySQL              | PostgreSQL |
| ------------ | ----------------- | ------------------ | ---------- |
| Large text   | `CLOB`            | `TEXT`, `LONGTEXT` | `TEXT`     |
| Binary large | `BLOB`            | `BLOB`, `LONGBLOB` | `BYTEA`    |
| Raw binary   | `RAW`, `LONG RAW` | `BINARY(n)`        | `BYTEA`    |

---

## 🔘 5. Boolean Types

| Oracle                            | MySQL                     | PostgreSQL  |
|----------------------------------|----------------------------|-------------|
| No native boolean (use `CHAR(1)` or `NUMBER(1)`) | `BOOLEAN` (`TINYINT(1)`) | `BOOLEAN`   |

---

## 🔄 6. Auto-Increment Columns

| Oracle                               | MySQL            | PostgreSQL                        |
| ------------------------------------ | ---------------- | --------------------------------- |
| `SEQUENCE` + `TRIGGER` or `IDENTITY` | `AUTO_INCREMENT` | `SERIAL`, `BIGSERIAL`, `IDENTITY` |


SOME - used with subquery if the