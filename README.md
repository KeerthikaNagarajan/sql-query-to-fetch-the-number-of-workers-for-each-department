# Ex-02:
## SQL QUERY TO FETCH THE NO OF WORKERS FOR EACH DEPARTMENT IN DESCENDING ORDER FROM THE SAMPLE DATA
### AIM:
To perform sql query to fetch the number of workers for each department in descending order from the sample data.
### ALGORITHM:
1. Create a table named worker with required columns.
2. Insert the values inside the table.
3. Select the department column from the table.
4. Count the number for distinct values as number of workers in each department.
5. Sort the number of workers in descending oder.
6. Display the output.
### PROGRAM:
```sql
CREATE TABLE worker (
    id INT,
    name VARCHAR(50),
    age INT,
    salary INT,
    department VARCHAR(50)
);
INSERT INTO worker (id, name, age, salary, department)
VALUES
    (1, 'John', 30, 5000.00, 'IT'),
    (2, 'Jane', 25, 4500.00, 'HR'),
    (3, 'Mike', 35, 6000.00, 'Sales'),
    (4, 'Sarah', 28, 5500.00, 'IT'),
    (5, 'David', 32, 5200.00, 'Marketing');
    
SELECT department, COUNT(*) AS no_of_workers
FROM worker
GROUP BY department
ORDER BY no_of_workers DESC;
```
### OUTPUT:
![2](https://github.com/KeerthikaNagarajan/EX-02-SQL/assets/93427089/54e251c3-9463-4fa4-a026-63621cddb222)

### RESULT:
Thus, sql query to fetch the number of workers for each department in descending order from the sample data is executed successfully.

