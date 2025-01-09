
# Employee Tablosu SQL İşlemleri

Bu README, bir veritabanındaki employee tablosu için SQL işlemlerini içermektedir.

## Tablo Yapısı

`employee` tablosunun yapısı şu şekildedir:

| Sütun Adı  | Veri Tipi    |
|------------|--------------|
| id         | INTEGER      |
| name       | VARCHAR(50)  |
| birthday   | DATE         |
| email      | VARCHAR(100) |

## SQL İşlemleri

### 1. Güncelleme İşlemleri

`employee` tablosundaki kayıtları güncellemek için kullanılan SQL sorguları:


```sql
UPDATE employee
SET name = 'Updated Name'
WHERE id = 1;
```


```sql
UPDATE employee
SET email = 'updatedemail@example.com'
WHERE name = 'Alice Johnson';
```


```sql
UPDATE employee
SET name = 'Birthday Update'
WHERE birthday = '1985-05-23';
```


```sql
UPDATE employee
SET birthday = '2000-01-01'
WHERE email = 'johndoe@example.com';
```


```sql
UPDATE employee
SET email = 'anotherupdate@example.com'
WHERE id = 50;
```

### 2. Silme İşlemleri

`employee` tablosundaki kayıtları silmek için kullanılan SQL sorguları:


```sql
DELETE FROM employee
WHERE id = 2;
```


```sql
DELETE FROM employee
WHERE name = 'Jane Smith';
```


```sql
DELETE FROM employee
WHERE birthday = '1992-07-14';
```


```sql
DELETE FROM employee
WHERE email = 'alicejohnson@example.com';
```


```sql
DELETE FROM employee
WHERE id = 50;
```

