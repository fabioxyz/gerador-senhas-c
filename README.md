# Password Generator · C Exercise

A Windows console exercise that generates batches of random strings and writes them to a text file.

**C · Windows · Strings and file I/O**

## Features

- Choose a length of up to **30 characters**.
- Generate up to **100 strings** in one batch.
- Use letters only, or letters and digits.
- Export the results to `senhasGeradas.txt`.

The console prompts are in Portuguese.

## Learning focus

Character arrays, indexing, input validation, pseudorandom generation and writing text files.

## Build and run

Use a Windows C toolchain such as MinGW-w64. The source includes `windows.h` and uses `Sleep()`. Add `#include <stdlib.h>` and `#include <time.h>` to declare the standard functions used by the program.

```powershell
gcc main.c -o gerador-senhas.exe
.\gerador-senhas.exe
```

## Project status

Educational only. The program uses time-seeded `rand()`, which is not cryptographically secure; generated strings should not be used as real account passwords. Results are saved as plain text.

[Browse all C projects](https://github.com/fabioxyz/projetos-c)
