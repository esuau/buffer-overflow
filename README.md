# Buffer Overflow

A simple program written in C to experiment Buffer Overflow attacks.

## Compile

```bash
$ gcc binary.c -o binary
```

## Execute

```bash
$ ./binary $(perl -e 'print "A"x200')
```