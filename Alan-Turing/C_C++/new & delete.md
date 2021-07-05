
### example
````c++
int* ptr;
ptr = new int;
delete ptr;
````

### What if I overwrite the pointer?
memory leak,
the previous spaces in memory aren't linked to a variable and still there occupying space.

## new Arrays
````c++
int* ptr;
ptr = new int[30]
delete []ptr; // am gonna erase... an array!, and this starts... at ptr!

int col=3;
int fil=2;
int A(fil)(col); // this works in c++17 and not all compilers accept this.
````
## new 2D arrays
````c++
int fil = 3;
int col = 5;
int **p;
new int*[fil];
for(int i = 0; i < fil; i++)
{
	p[i] = new int[col];
}
````
you can access them like any other array.
if you want to iterate exactly as an array, you should.
````c++
for(int*q[fil]= p; q < p+fil; q++)
{
	for(int*j=*q; j < *(q+1); j++)
	{
		// Do something
	}
}
the array is now in heap and not in stack
````




