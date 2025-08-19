# ft_printf

<img width="1200" height="631" alt="image" src="https://github.com/user-attachments/assets/484bbb17-79db-4ada-b0c3-7cdc2c7e7ed3" />

### Description

This project is a basic replica of the libc `printf()` function, implemented as part of the 42 Cursus. It supports a subset of the standard `printf()` specifiers to format and print data to the standard output.

#### Supported Specifiers
- `%c` - Prints a single character
- `%s` - Prints a string
- `%p` - Prints a pointer address
- `%d` or `%i` - Prints a signed integer
- `%u` - Prints an unsigned integer
- `%x` or `%X` - Prints an unsigned integer in hexadecimal format

### Installing and Running the Project

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/42_ft_printf
   ```
2. Run `make` to compile the library:
   ```bash
   make
   ```
3. Run `make clean` to remove unnecessary object files:
   ```bash
   make clean
   ```
4. Compile your project (e.g., `main.c`) with the generated `libftprintf.a`:
   ```bash
   cc -Wall -Wextra -Werror main.c libftprintf.a
   ```

### Makefile

The `ft_printf()` project is an extension of the [Libft](https://github.com/your-username/42_Libft) library. The provided Makefile compiles both `ft_printf` and `Libft` together into `libftprintf.a`.

#### Available Targets
- `make` or `make all`: Builds the `libftprintf.a` library.
- `make clean`: Deletes all object files.
- `make fclean`: Deletes `libftprintf.a` and all object files.
- `make re`: Deletes everything and rebuilds `libftprintf.a`.

#### Inspecting the Library
To check the contents of `libftprintf.a`, run:
```bash
ar -t libftprintf.a
```

### Tests
This project has been tested using [printfTester](https://github.com/Tripouille/printfTester).

### Disclaimer
At [42 School](https://en.wikipedia.org/wiki/42_(school)), projects must adhere to the "Norm," the school's coding standard. This may result in implementations that seem unconventional but are designed to meet the Norm's requirements.
