# overflow.c

This is a simple program causing a segmentation fault.

## Compile

```bash
$ gcc overflow.c -o overflow -fno-stack-protector
```

## Execute

```bash
$ ./overflow
```

## Expected result

```bash
Segmentation fault (core dumped)
```
