**Exercise 1-2.** Experiment to find out what happens when printf's argument
string contains \c, where c is some character not listed above.
```c
/* hello.c */
#include <stdio.h>

main()
{
    printf("hello, world\d");
}
```
When we try to compile it, compiler outputs a warning:
```sh
hello.c: In function ‘main’:
hello.c:5:28: warning: unknown escape sequence: '\d'
```
