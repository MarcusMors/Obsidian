

### prototype

	void * malloc (size-t, size);

#### example

	int* a,b;
	a = (int*) malloc(20 * sizeof(int));
	b = (int*) calloc(20,sizeof(int));
	

garbage collector looks for unused memory spaces to free them.

what if malloc doesn't find the required space?
malloc returns a null pointer.


![[malloc vs calloc.svg]]