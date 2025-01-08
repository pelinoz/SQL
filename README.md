
# Employee Table SQL Operations

This README provides SQL operations for an employee table in a relational database.

## Table Structure

The `employee` table has the following structure:

| Column Name | Data Type   |
|-------------|-------------|
| id          | INTEGER     |
| name        | VARCHAR(50) |
| birthday    | DATE        |
| email       | VARCHAR(100)|

## SQL Operations

### 1. Update Operations

The following SQL queries update records in the `employee` table:

#### Update Name by ID

```sql
UPDATE employee
SET name = 'Updated Name'
WHERE id = 1;
```

#### Update Email by Name

```sql
UPDATE employee
SET email = 'updatedemail@example.com'
WHERE name = 'Alice Johnson';
```

#### Update Name by Birthday

```sql
UPDATE employee
SET name = 'Birthday Update'
WHERE birthday = '1985-05-23';
```

#### Update Birthday by Email

```sql
UPDATE employee
SET birthday = '2000-01-01'
WHERE email = 'johndoe@example.com';
```

#### Update Email by ID

```sql
UPDATE employee
SET email = 'anotherupdate@example.com'
WHERE id = 50;
```

### 2. Delete Operations

The following SQL queries delete records from the `employee` table:

#### Delete by ID

```sql
DELETE FROM employee
WHERE id = 2;
```

#### Delete by Name

```sql
DELETE FROM employee
WHERE name = 'Jane Smith';
```

#### Delete by Birthday

```sql
DELETE FROM employee
WHERE birthday = '1992-07-14';
```

#### Delete by Email

```sql
DELETE FROM employee
WHERE email = 'alicejohnson@example.com';
```

#### Delete by ID

```sql
DELETE FROM employee
WHERE id = 50;
```

## Usage

- Run the above queries on your database system to perform the respective update or delete operations.
- Replace the values in the queries (such as name, birthday, email, id) to fit your specific needs.
