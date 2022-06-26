**Exercise 1-1.** Run the "hello, world" program on your system. Experiment
with leaving out parts of the program, to see what error messages you get.
```c
/* hello.c */
#include <stdio.h>

main()
{
    printf("hello, world\n")
}
```
To run this programm, we need to compile it first:
```bash
cc hello.c
```
After this, we get an executable named `a.out`. We can run it now:
```bash
./a.out
```
At the result, we get our `hello, world` line as output.

Without `#include <>` compiler warn us:
```bash
hello.c: In function ‘main’:
hello.c:5:5: warning: implicit declaration of function ‘printf’ [-Wimplicit-function-declaration]
    5 |     printf("hello, world\n");
      |     ^~~~~~
hello.c:1:1: note: include ‘<stdio.h>’ or provide a declaration of ‘printf’
  +++ |+#include <stdio.h>
    1 | 
hello.c:5:5: warning: incompatible implicit declaration of built-in function ‘printf’ [-Wbuiltin-declaration-mismatch]
    5 |     printf("hello, world\n");
      |     ^~~~~~
hello.c:5:5: note: include ‘<stdio.h>’ or provide a declaration of ‘printf’
``` 
