you can create one using classes or structures

### Differences between classes and structures
by default, everything in a class is private.
by default, everything in a struct is public

## Struct

````c++
struct node
{
	int value;
	node *next;
}
````

We use them like this:
````c++
node* head;
head = new node;
(*head).value = 1;
head->value = 1;
head->next = new node;
head->next->value = 2;
head->next->next = new node;
head->next->next->value = 3;
head->next->next->next = nullptr;
````

double way linked list
````c++
struct node
{
	int value;
	node *next, *prev;
}
````
binary tree
````c++
struct node
{
	int value;
	node  *left,*right;
}
````
graphs
````c++
struct node
{
	int value;
	node  *left,*right;
}
````

with constructor
````c++
struct node
{
	int value;
	node* next;
	node(int v, node* n = nullptr)
	{
		valor = v;
		next = n;
	}
}
class node
{
public:
	int value;
	node* next;
	node(int v, node* n = nullptr)
	{
		valor = v;
		next = n;
	}
}

````

- [ ] a
- [ ] b
- [ ] c


## linked lists
sorted without repetition.

### attributes
- head -> node*

### methods
- add
- delete
- bool find(key, node*& position){return nullptr if pos = 0 or head, usually return the one before the position} //used by add and delete
- print 






