### Start by updating the packages list:
    sudo apt update

### Install the build-essential package by typing:
    sudo apt install build-essential
The command installs a bunch of new packages including gcc, g++ and make.

### You may also want to install the manual pages about using GNU/Linux for development:
    sudo apt-get install manpages-dev

### To validate that the GCC compiler is successfully installed, use the gcc --version command which prints the GCC version:
    gcc --version

# Compiling a Hello World Example

Compiling a basic C or C++ program using GCC is pretty easy. Open your text editor and create the following file:

    nano hello.c

    #include <stdio.h>
    int main()
    {
      printf ("Hello World!\n");
      return 0;
    }

### Save the file and compile it into an executable using the following command:

    gcc hello.c -o hello

This will create a binary file named hello in the same directory where you run the command.

### Execute the hello program with:

    ./hello

### The program should print:

    Hello World!
