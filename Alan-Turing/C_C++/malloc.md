memory allocation

### prototype

	void * malloc (size-t size);

#### example

	char* buffer;
	buffer = (char*) malloc(100);
	if(buffer == NULL) return 0
	*buffer = 'a'
	free(buffer);

garbage collector looks for unused memory spaces to free them.

what if malloc doesn't find the required space?
malloc returns a null pointer.
