>[!faq] first question
>the function insert(index,value);
>take order of N ==>O(n)

---
>[!faq]
>Arrays have better cache locality than a linked list. True or False?
> ==> True
> >[!note]
> >Keep it as note for future about 'locality of reference' or google and learn. [why-does-cache-locality-matter-for-array-performance](https://stackoverflow.com/questions/12065774/why-does-cache-locality-matter-for-array-performance)

---
>[!info]
>We can operator overload [] for a linked list. However, we still have to do O(n) iteration. No random access in linked list. This is different from the syntax of operator.

---
![[ArcoLinux-2023-11-08-1699439702_screenshot_1920x1080.jpg]]

![[ArcoLinux-2023-11-08-1699439706_screenshot_1920x1080.jpg]]


---
>[!faq]
>Let's say our current list is:
>25 -> 20 -> 15 -> 7 -> 10
>
>1- What is the output of this function f() call?
>
>2- Guess what does this function does

```cpp
bool f(Node* node) {
	return !node || !node->next || node->data > node->next->data && f(node->next);
}
bool f() {
	return f(head);
}
```
 >[!answer]
 >- [ ] 1
 >- [x] 0
 >- [ ] error

---
>[!faq]
>Assume we have list: 1 2 3 4 5 6 7 8
>
>If we call f(), what is the last value for cnt variable before a crash?
>Answer ==>6

```cpp
void f() {
	int cnt = 0;
	while(head) {
		++cnt;
		cout<<cnt<<flush<<"\n";
		head->data += head->next->next->next->data;
		head = head->next;
	}
}
```

---
>[!faq]
>A logical data structure focuses on storing data in the memory in a specific way. True or False?
>==>False

---
>[!faq]
>If there is no deletion, and most of the insertions happen in the end and in total ==we have a small number of elements==, probably vector is a better choice. True or False
>==>True

>[!faq]
>If there is no deletion, and most of the insertions happen in the end but in total, ==we have a huge number of elements==, probably vector is a better choice. True or False
>==>False

