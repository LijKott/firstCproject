# C Programming - Compilation Guide

## Basic Compilation

Compile a single C file:
```bash
gcc hello.c -o hello
```

Run the program:
```bash
./hello
```

## Common GCC Commands

Compile with warnings enabled (recommended):
```bash
gcc -Wall hello.c -o hello
```

Compile with debugging symbols (for use with gdb):
```bash
gcc -g hello.c -o hello
```

Compile with optimization:
```bash
gcc -O2 hello.c -o hello
```

Compile multiple files:
```bash
gcc main.c utils.c -o program
```

## Useful Flags

- `-Wall` - Enable all warnings
- `-Wextra` - Enable extra warnings
- `-g` - Include debugging information
- `-O2` - Optimize code (level 2)
- `-o filename` - Name the output file
- `-c` - Compile without linking (creates .o file)
- `-std=c11` - Use C11 standard
- `-lm` - Link math library

## Examples

Compile with all warnings and debugging:
```bash
gcc -Wall -Wextra -g hello.c -o hello
```

Compile with C11 standard:
```bash
gcc -std=c11 -Wall hello.c -o hello
```

## Clean Up

Remove compiled executable:
```bash
rm hello
```

Remove all executables and object files:
```bash
rm -f *.o hello
```

## Troubleshooting

Check GCC version:
```bash
gcc --version
```

Check if GCC is installed:
```bash
which gcc
```

View compilation errors in detail:
```bash
gcc -Wall -Wextra hello.c -o hello 2>&1 | less
```
