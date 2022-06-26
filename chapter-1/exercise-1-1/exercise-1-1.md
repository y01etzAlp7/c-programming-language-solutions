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
```sh
cc hello.c
```
After this, we get an executable named `a.out`. We can run it now:
```sh
./a.out
```

