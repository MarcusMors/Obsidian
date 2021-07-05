memory reallocation

## Prototype
	void * reallocation(void* ptr, size-t size);

## Example
	int *a;
	a = (int*) malloc(20 * sizeof(int));
	a[0] = 10;
	a[10] = 20;
	a[19] = 200;
	b = (int*) realloc(a, 50 * sizeof(int));

3 options:
* contiguous memory is available, b_ptr = a_ptr
* contiguous memory isn't available, b_ptr != a_ptr, and the memory location of a_ptr is set to free
* b is set to NULL, no memory available. Rare case

### equivalence to malloc

	int* a = (int*) malloc(20 * sizeof(int));

Has the same result as; 
	
	int *b = nullptr;
	b = (int*) realloc(b, 20 * sizeof(int));


