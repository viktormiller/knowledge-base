# Commands

## Save MySQL query results to a file

There are several ways to save the results to a file:

### 1. SELECT INTO OUTFILE (recommended for large amounts of data)

```sql
SELECT id FROM table_name INTO OUTFILE ‘/tmp/output.txt’;
```

#### With formatting: 

```sql
SELECT id FROM table_name INTO OUTFILE ‘/tmp/output.txt’ FIELDS TERMINATED BY ‘,’ ENCLOSED BY ‘“’ LINES TERMINATED BY ‘\n’;
```

Important:

- The MySQL server must have write permissions for the directory 
- The path must be absolute
- The file must not already exist

### 2. Command line with redirection

```bash
mysql -u username -p -D database_name -e “SELECT id FROM table_name;” > output.txt
```

#### Without header and formatting: 

```bash
mysql -u username -p -D database name -N -B -e “SELECT id FROM table_name;” > output.txt
```

Options:

- `-N` : No column headers
- `-B` : Batch mode (tab-separated)

## 3. mysqldump for CSV export

```bash
mysql -u username -p -D database_name -B -e “SELECT id FROM table_name;” | sed ‘s/\t/,/g’ > output.csv
```
