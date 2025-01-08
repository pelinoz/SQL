
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

#### ID'ye Göre Name Güncelleme

```sql
UPDATE employee
SET name = 'Updated Name'
WHERE id = 1;
```

#### Name'e Göre Email Güncelleme

```sql
UPDATE employee
SET email = 'updatedemail@example.com'
WHERE name = 'Alice Johnson';
```

#### Birthday'e Göre Name Güncelleme

```sql
UPDATE employee
SET name = 'Birthday Update'
WHERE birthday = '1985-05-23';
```

#### Email'e Göre Birthday Güncelleme

```sql
UPDATE employee
SET birthday = '2000-01-01'
WHERE email = 'johndoe@example.com';
```

#### ID'ye Göre Email Güncelleme

```sql
UPDATE employee
SET email = 'anotherupdate@example.com'
WHERE id = 50;
```

### 2. Silme İşlemleri

`employee` tablosundaki kayıtları silmek için kullanılan SQL sorguları:

#### ID'ye Göre Silme

```sql
DELETE FROM employee
WHERE id = 2;
```

#### Name'e Göre Silme

```sql
DELETE FROM employee
WHERE name = 'Jane Smith';
```

#### Birthday'e Göre Silme

```sql
DELETE FROM employee
WHERE birthday = '1992-07-14';
```

#### Email'e Göre Silme

```sql
DELETE FROM employee
WHERE email = 'alicejohnson@example.com';
```

#### ID'ye Göre Silme

```sql
DELETE FROM employee
WHERE id = 50;
```

