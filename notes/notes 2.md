data base
- accuracy
- integrity
- limits
- scalability
- maintenance
- security
DB system vs file system
1. duplication
2. search is linear
3. no constrains
4. no relations
5. manual recovery
6. security & permissions
7. no standard

---
switch between data bases
![[Pasted image 20241028203055.png]]

---
### data base life cycle
1. analysis -> system analyst
	. requirement document
2. database design -> database designer
	. entity relationship diagram `ERD`
3. data base mapping -> database designer
	. data base schema
4. database implementation -> database developer
	. using DBMS (SQL server) to create database
5. application -> developer
	. web-desktop-mobile
6. client -> end user
	. use database indirectly through the app
---
### the ER model
1. entities - person, place, object, event, concept(often corresponds to a real time object that is unique)
2. attributes - property or characteristic of an entity type
3. relationships - link between entities (corresponds to primary key-foreign key)
strong entity `primary key`
weak entity `partial key - dependent`
#### Relationships
- simple
- composite : `birth year month day`
- derived : `calculated like yearly salary`
- multi valued `more than one address`
- complex attribute `multi valued + composite`
- recursive relationship (unary, binary, ternary)
#### Mapping cardinalities
- one to one `employee own car`
- one to many  `department has employee`
- many to many `course take student`
	- one to many course has student
	- many to one student have courses
#### participation constraint
- employee must be in a department `total`
- employee manages a department `partial`
