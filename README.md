# Template Project

This project is a template for C projects using the GNU GPL v3. You can fork it, copy it, whatever. It's handy.

# Commands

This template project is meant to be a standard for my projects. While in the project's root, one can input:

    $ make         #Compile the project and output an executable in ./bin
    $ make clean   #Remove all .o files in ./bin/obj
    $ make fclean  #Same as "make clean" but also removes all compiled executables
    $ make re      #Same as "$ make fclean && make"

# Variables

This template is modular. As such, the project's name can be changed by setting the variable `NAME` in `./Makefile` at line `16`. The compiler warnings and flags can also be changed in lower lines.

# Folder tree

- `BIN_DIR` (Default: `./bin`) contains the compiled executable, named with a timestamp and `.bin` extension.
- `OBJ_DIR` (Default: `./bin/obj`) contains the object files produced by the C compiler.
- `SRC_DIR` (Default: `./sources`) contains the source (`.c`) files. All .c files located in this directory or subdirectories will be compiled in object files.
- `HDR_DIR` (Default: `./headers`) contains the header (`.h`) files. All .h files in this directory can be included using `#include <file.h>` by the source files.
