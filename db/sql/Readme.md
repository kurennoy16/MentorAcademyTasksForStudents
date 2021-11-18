# Task SQL DBs

Create a DB and the following tables:

```
CREATE TABLE employee
(
    id BIGSERIAL PRIMARY KEY,
    name varchar(100)
);

CREATE TABLE salary
(
    id BIGSERIAL PRIMARY KEY,
    employee_id int,
    name varchar(100),
    CONSTRAINT salary_employee_id_fkey FOREIGN KEY (employee_id) REFERENCES employee (id)
);
```

## Create repository and implement the following methods:
* Retrieve the list of employees
* Retrieve the list of salary records
* Add employee

### Bonus points:
* Add salary record 
* Implement using different libraries (`gorm`, `sqlc`, `sqlx`, `ent`)
