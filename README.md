# SQL Exercises

## Topics

- Structured Query Language (SQL)
- Relational Databases
- SQLite
- Writing Basic Queries

## Assignment

For this lab you will:

- write SQL statements against a pre-populated database using an online tool. Once you have the correct SQL Statement for each query, write it inside the `queries.md` file under the appropriate heading.
- install [`SQLite Studio`](https://sqlitestudio.pl/index.rvt) and use it to create a database.
- using `SQLite Studio` add a table to the database you just created.

### Write Basic Queries

Visit [SQL Try Editor at W3Schools.com](https://www.w3schools.com/Sql/tryit.asp?filename=trysql_select_top) using the **Google Chrome (or Chromium if you use Linux) browser** and write _SQL queries_ for the following requirements:

- [x] find all customers that live in London. Returns 6 records.
- [x] find all customers with postal code 1010. Returns 3 customers.
- [x] find the phone number for the supplier with the id 11. Should be (010) 9984510.
- [x] list orders descending by the order date. The order with date 1997-02-12 should be at the top.
- [x] find all suppliers who have names longer than 20 characters. You can use `length(SupplierName)` to get the length of the name. Returns 11 records.
- [x] find all customers that include the word "market" in the name. Should return 4 records.
- [x] add a customer record for _"The Shire"_, the contact name is _"Bilbo Baggins"_ the address is _"1 Hobbit-Hole"_ in _"Bag End"_, postal code _"111"_ and the country is _"Middle Earth"_.
- [x] update _Bilbo Baggins_ record so that the postal code changes to _"11122"_.

**Clicking the `Restore Database` button in the page will repopulate the database with the original data and discard all changes you have made**.

### Create Database and Table

- [x] use [`SQLite Studio`](https://sqlitestudio.pl/index.rvt) to create a database, name it `budget.sqlite3`.
- [x] add an `accounts` table with the following _schema_:

  - [x] `id`, numeric value with no decimal places that should autoincrement.
  - [x] `name`, string, add whatever is necessary to make searching by name faster.
  - [x] `budget` numeric value.

- [x] constraints
  - [x] the `id` should be the primary key for the table.
  - [x] account `name` should be unique.
  - [x] account `budget` is required.

## Stretch Problems

- [x] list orders grouped by customer showing the number of orders per customer. _Rattlesnake Canyon Grocery_ should have 7 orders.
- [x] list customers names and the number of orders per customer. Sort the list by number of orders in descending order. _Ernst Handel_ should be at the top with 10 orders followed by _QUICK-Stop_, _Rattlesnake Canyon Grocery_ and _Wartian Herkku_ with 7 orders each.
- [x] list orders grouped by customer's city showing number of orders per city. Returns 58 Records with _Aachen_ showing 2 orders and _Albuquerque_ showing 7 orders.
- [x] delete all customers that have no orders. Should delete 17 (or 18 if you haven't deleted the record added) records.
