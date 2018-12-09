# Buffer Overflow

A few programs written in C to experiment Buffer Overflow attacks.

## Prerequisites

There are two prerequisites when running these programs on Linux.

### Disable ASLR

```bash
$ sudo bash -c 'echo 0 > /proc/sys/kernel/randomize_va_space'
```

### Disable canaries

```bash
$ gcc <program_name>.c -o <program_name> -fno-stack-protector
```