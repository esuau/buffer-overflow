# Buffer-Overflow Vulnerability

Source: http://www.cis.syr.edu/~wedu/seed/Labs_12.04/Vulnerability/Buffer_Overflow/

# Compile

Compile the code that launches a shell.

```bash
$ gcc -z execstack -o call_shellcode call_shellcode.c
```

Compile the vulnerable program. You have to log in as `root` to make it `set-root-uid`.

```
$ su root 
Password (enter root password) 
# gcc -o stack -z execstack -fno-stack-protector stack.c 
# chmod 4755 stack # exit
```

Compile the program that exploits the vulnerability.

```bash
$ gcc -o exploit exploit.c 
```

# Execute

Create the badfile.

```bash
$ ./exploit
```

Launch the attack.

```bash
$./stack
```

You now have a root shell.

```
# 
``` 