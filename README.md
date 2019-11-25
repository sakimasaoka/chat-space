# README
変更しました

mysql> SHOW columns FROM ress;
+----------+--------------+------+-----+---------+-------+
| Field    | Type         | Null | Key | Default | Extra |
+----------+--------------+------+-----+---------+-------+
| id       | int(11)      | YES  |     | NULL    |       |
| users_id | int(11)      | YES  |     | NULL    |       |
| text     | varchar(255) | YES  |     | NULL    |       |
| time     | datetime     | YES  |     | NULL    |       |
| tweet_id | int(11)      | YES  |     | NULL    |       |
+----------+--------------+------+-----+---------+-------+
5 rows in set (0.00 sec)

mysql> SHOW columns FROM tweet;
+------------+--------------+------+-----+---------+-------+
| Field      | Type         | Null | Key | Default | Extra |
+------------+--------------+------+-----+---------+-------+
| id         | int(11)      | YES  |     | NULL    |       |
| users_id   | int(11)      | YES  |     | NULL    |       |
| text       | varchar(255) | YES  |     | NULL    |       |
| group_name | varchar(255) | YES  |     | NULL    |       |
| time       | datetime     | YES  |     | NULL    |       |
| image      | varchar(255) | YES  |     | NULL    |       |
+------------+--------------+------+-----+---------+-------+
6 rows in set (0.01 sec)

mysql> SHOW columns FROM users;
+------------+--------------+------+-----+---------+-------+
| Field      | Type         | Null | Key | Default | Extra |
+------------+--------------+------+-----+---------+-------+
| id         | int(11)      | YES  |     | NULL    |       |
| name       | varchar(255) | YES  |     | NULL    |       |
| email      | varchar(255) | YES  |     | NULL    |       |
| password   | varchar(255) | YES  |     | NULL    |       |
| group_name | varchar(255) | YES  |     | NULL    |       |
+------------+--------------+------+-----+---------+-------+
This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...
