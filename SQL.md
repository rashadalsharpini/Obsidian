```sql
select * from celebs;
```
the * is a sign that means every column within the table

---

```sql
create table celebs (
	id integer,
	name text,
	age integer
);
```
1. `create table` is a clause that tells SQL you want to create a new table.
2. celebs is the name of the table.
3. `(id integer, name text, age integer)` is a list of parameters defining each column,
or attribute in the table and its data type.

---

```sql
insert into celebs (id, name, age)
values (1, "rashad", 20);
```
the `insert into` statement inserts a new row into a table.
we can use the `insert` statement when you want to add new records.

---

```sql
select name from celebs;
```
`select` statements are used to fetch data from a database. in the statement, `select` returns all data in the `name` column of the `celebs` table.

---

```sql
alter table celebs
add column twitter_handle text;
```
the `alter table` statement adds a new column to a table.
1. `alter table` is a clause that lets you make the specified changes.
2. `celebs` is the name of the table that is being changed.
3. `add column` is a clause that lets you add a new column to a table
	 - `twitter_handle` is the name of the new column being added
	 - `text` is the date type.
 1. `null` is a special value in SQL that represents missing or unknown date.

---

```sql
update celebs
set twitter_handle = '@taylor'
where id = 4;
```
the `update` statement edits a row in a table.
the `where` statement is a clause that indicates which row(s) to update with the new
column value.

---

```sql
delete from celebs
where twitter_handle is null;
```
the `delete from` statement deletes one or more rows from a table. 
`is null` is a condition in SQL that returns true when the value is null and false otherwise.

---

```sql
create table celebs (
	id integer primary key,
	name text unique,
	date_of_birth text not null,
	date_of_death text default 'not applicable'
);
```
Constraints that add information about how a column can be used are invoked after
specifying the data type for a column. They can be used to tell the database to reject
inserted data that does not adhere to a certain restriction.

1. `primary key` columns can be used to uniquely identify the row. attempts to insert a row with identical value to a row already in the table will result in a constrain violation which will not you to insert the new row.
2. `unique` columns have a different value for every row. this is similar to `primary key` except a table can have many different `unique` columns.
3. `not null` must have a value. attempts to insert a row without a value for a `not null` column will result in a constrain violation and the new row will not be inserted.
4. `default` columns take an additional argument that will be the assumed value for an inserted row if the row does specify a value for that column.
