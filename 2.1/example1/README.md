# binary.c

This is a simple program causing a segmentation fault.

## Compile

```bash
$ gcc binary.c -o binary -fno-stack-protector
```

## Execute

No error at this point.

```bash
$ ./binary AAA
AAA
```

The following causes a segmentation error.

```bash
$ ./binary $(perl -e 'print "A"x200')
Segmentation fault (core dumped)
```
