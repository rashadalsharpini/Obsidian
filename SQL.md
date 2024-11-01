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

---

back to the `select` statement you could chose more than a column
```sql
select name, genre
from movies;
```

`as` is a keyword in sql that allows you to rename a column or table using an alias.
the new name can be anything you want as long as you put it inside of single quotes. 
```sql
select name as 'title' from movies;
```
>[!note]
> . although it's not always necessary, it's considered best practice to surround your aliases with sing quotes.
> 	. note that this practice is specific to SQLite, the RDBMS used in this exercise. when you work with other RDBMS, notably PostgreSQL, no quotes or double quotes may be required in place of single quotes.
> . when using `as`, the columns are not being renamed in the table. 
> the aliases only appear in the result.

by adding `distinct` before the column name,the values will not be repeated. which means that it will return unique values only!
```sql
select distinct year from movies;
```

---
Comparison operators used with the `WHERE` clause are:

- `=` equal to
- `!=` not equal to
- `>` greater than
- `<` less than
- `>=` greater than or equal to
- `<=` less than or equal to

---
`like` can be a useful operator when you want to compare similar values.
the movies table contains to films with similar titles seven se7en.
```sql
select * from movies
where name like 'Se_en';
```
the `_` means you can substitute any individual character here without breaking the pattern.

the `%` is another wildcard character that can be used.
```sql
select * from movies
where name like 'A%';
```
- `A%` matches all movies with name that begin with 'A'.
- `%a` matches all movies with name that ends with 'a'.
we can use this pattern both before and after.
```sql
select * from movies
where name like '%man%';
```

---

Unknown values indicated by `null`.
it's not possible to test for null values with comparison operators, such as = or != .
instead, we will have to use these operators:
- `is null`
- `is not null`
```sql
select name from movies
where imdb_rating is not null;
```

---

```sql
select * from movies
where year between 1990 and 1999;
```
that will give you the information from 1990 up to 1999 included.
```sql
select * from movies
where name between 'A' and 'J';
```
in this statement, `between` filters the result set to only include movies with `name`s that begin with the letter 'A' up to,
but not including the ones that begin with 'J'.
However, if movies has a name of simply 'J', it would be actually match. this is because `between` goes up to the second value - up to 'J'. So the movie named 'J' would be included in the result set but not 'Jaws'.

---

you can make more than one condition like 
```sql
select * from movies
where year between 1990 and 1999 and genre = 'romance';
```
and as you know the `and` won't return a value unless the conditions are true all of them.
but not like the `or` it will return a value if any condition is true.
```sql
select * from movies
where year > 2014 or genre = 'action';
```

---

```sql
select * from movies
order by name;
```
- `order by` is a clause that indicates you want to sort the result set by a particular column.
- `decs` is a keyword used in `order by` to sort the in decreasing order high to low z to a.
- `asc` is a keyword used in `order by` to sort the in ascending order low to high a to z. 
>[!note] order by always comes after where (if where is present).

---

we have been working with a fairly small table fewer than 250 row,
but most sql tables contains hundreds of thousands of records.
for instance, imagine that we just want to see a few examples of records.
```sql
select * from movies
limit 10;
```
`LIMIT` always goes at the very end of the query. Also, it is not supported in all SQL databases.

---

```sql
select name
	case
		when imdb_rating > 8 then 'fantastic'
		when imdb_rating > 6 then 'poorly received'
		else 'avoid at all costs'
	end
from movies;
```
- Each `WHEN` tests a condition and the following `THEN` gives us the string if the condition is true.
- The `ELSE` gives us the string if _all_ the above conditions are false.
- The `CASE` statement must end with `END`.

---

