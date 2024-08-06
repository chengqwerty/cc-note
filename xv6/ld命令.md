
## 常用命令

```shell
ld /usr/lib/x86_64-linux-gnu/crt1.o /usr/lib/x86_64-linux-gnu/crti.o /usr/lib/x86_64-linux-gnu/crtn.o  -o test -L. -Bstatic -lmath -lc test.o --dynamic-linker /lib64/ld-linux-x86-64.so.2

ld -o hello4 /usr/lib/x86_64-linux-gnu/crt1.o /usr/lib/x86_64-linux-gnu/crti.o hello.o -lc /usr/lib/x86_64-linux-gnu/crtn.o --dynamic-linker /lib64/ld-linux-x86-64.so.2

gcc -### -static -o hello3 hello.c

gcc -###  -o hello3 hello.c

ld /usr/lib/x86_64-linux-gnu/crt1.o /usr/lib/x86_64-linux-gnu/crti.o /usr/lib/x86_64-linux-gnu/crtn.o -o test test.o -L. -lmath -lc  --dynamic-linker /lib64/ld-linux-x86-64.so.2

ar -rc libmath.a math.o

gcc -c math.c

gcc -o test test.c -L. -static -lmath
```

