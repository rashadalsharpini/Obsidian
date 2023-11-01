The **"Template Titans"** challenge test your C++ template programming skills.
You'll create a versatile, efficient data structure and apply it in a real world app.
Deadline:{31-OCT-2023} {Personal Task}
![[ArcoLinux-2023-10-26-1698310673_screenshot_1920x1080.jpg]]

## Tasks
- Create a powerful **template container class** that can dynamically store elements of any data type. this class should be able to handle a wide range of data types including 
	1. integers
	2. strings
	3. objects
 it should also be **able to resize itself as needed** to accommodate new elements.
 - implement member functions to **insert** elements at
	 1. beginning
	 2. end
	 3. specific positions in the container
- create function to **remove** elements based on their **value or Postion** within 
the container
- include a function to **find** and **retrieve** elements based on **given value**.
- incorporate **sorting** algorithms for ordering elements in the container
- create additional functionalities like
	1. resizing
	2. capacity management
	3. batch operations for enhanced performance
- design iterator classes that provide seamless traversal of container elements
	- begin, end, next, prev

## Bonus
- implement additional operations like 
	1. reversing
	2. merging the container
- add support for range-based for loops to iterate through the container.
- ensure efficient memory management and error handling for edge cases.

---
## Real-World App {library management system}
Now, let's put your custom container to practical use in a real world app
a library management system. the system should allow the library staff to manage books efficiently.
## Application Features:
1. Book catalog: use your template container to store and manage book records
efficiently. Each book record should include details like
	1. title
	2. author
	3. ISBN
	4. genre
	5. availability status
2. Book insertion and removal: implement functions to add new books to the catalog
and remove books when they are returned or withdrawn.
3. Book search: create a search function to find books based on title, author, ISBN
or genre.
4. Book borrowing: implement a function that allows library members to borrow 
available books.
5. Book Sorting: utilize your sorting algorithms to arrange books in catalog by 
title, author, or genre for easy access.
6. Book statistics: provide statistical functions like the total number of books,
 available books, and borrowed books. book counter for every book

## Bonus
1. Add error handling and input validation to handle various scenarios gracefully.
2. Optimize the container implementation for memory efficiency and fast data access.
---
- [x] store and manage book records
- [x] insert
- [x] display
- [x] search
- [ ] sort
- [x] remove
- [x] statistics
- [x] borrow
---
- [ ] error handling
- [ ] binary search





