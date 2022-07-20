# sqlodev8
PAtika SQL Ödev-8

1- 
CREATE TABLE employee (
    id INTEGER PRIMARY KEY,
    name VARCHAR(50) NOT NULL,
    birthday DATE,
    email VARCHAR(100)
)

3-
UPDATE employee
SET name = 'NXXXXXX'
WHERE name LIKE 'N%'
RETURNING *

UPDATE employee
SET email = 'test@test.com'
WHERE email LIKE '%d%'
RETURNING *

UPDATE employee
SET name = 'deniz'
WHERE name = 'Wang'
RETURNING *

UPDATE employee
SET name = 'Dummy'
WHERE email = 'test@test.com'
RETURNING *

UPDATE employee
SET birthday = '1991-10-02'
WHERE name LIKE '%v%'
RETURNING *

4- 
DELETE FROM employee
WHERE email = 'test@test.com'

DELETE FROM employee
WHERE name = 'Dummy'
