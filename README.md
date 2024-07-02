# crud-ajax

Recuerda crear tu base de datos tareas.

```shell
# 1. go to apache folder and clone source code
cd /var/www/html
git clone

# 2. login to mysql and create DB, grant permissions to mysql user
sudo mysql -u root -p

mysql> create database tareas;
Query OK, 1 row affected (0.03 sec)

mysql> GRANT ALL ON tareas.* TO mvp_project@localhost;
Query OK, 0 rows affected (0.02 sec)

# 3. import SQL backup
mysql -u mvp_project -p tareas < tareas.sql

# 3.1. inspect DB
mysql -u mvp_project -p tareas

# 4. configure DB conexion
vim php/database.php

```
