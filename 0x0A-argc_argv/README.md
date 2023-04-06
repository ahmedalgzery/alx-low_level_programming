Introduction
This project covers the following topics:

How to use arguments passed to your program
Two prototypes of main and when to use them
How to use attribute((unused)) or (void) to compile functions with unused variables or parameters
Copyright and Plagiarism
Requirements
Allowed editors: vi, vim, emacs
All files will be compiled on Ubuntu 20.04 LTS using gcc, using the options -Wall -Werror -Wextra -pedantic -std=gnu89
All files should end with a new line
A README.md file, at the root of the folder of the project is mandatory
Code should use the Betty style. It will be checked using betty-style.pl and betty-doc.pl
Not allowed to use global variables
No more than 5 functions per file
Prototypes of all functions and _putchar should be included in header file called main.h
Don’t forget to push the header file
Allowed to use the standard library
How to Use Arguments Passed to Your Program
In C, arguments can be passed to your program through the command line. These arguments can be used by your program for various purposes. The main function takes two arguments: argc and argv. argc stands for argument count, and argv stands for argument vector. argc is an integer that represents the number of arguments passed to the program, including the name of the program itself. argv is an array of strings that contains the arguments passed to the program.

Here's an example of how to use arguments passed to your program:
#include <stdio.h>

int main(int argc, char *argv[])
{
    int i;
    for (i = 0; i < argc; i++)
    {
        printf("arg %d: %s\n", i, argv[i]);
    }
    return 0;
}

In this example, we iterate through the argv array and print out each argument along with its index.

Two Prototypes of Main and When to Use Them
There are two prototypes for the main function:
int main(void);
int main(int argc, char *argv[]);

The first prototype takes no arguments, while the second prototype takes two arguments: argc and argv.

You should use the first prototype (int main(void)) if your program does not need to accept any command-line arguments. You should use the second prototype (int main(int argc, char *argv[])) if your program needs to accept command-line arguments.

How to Use attribute((unused)) or (void) to Compile Functions with Unused Variables or Parameters
When compiling your program, you may encounter warnings about unused variables or parameters in your functions. To prevent these warnings, you can use the __attribute__((unused)) or (void) syntax.

Here's an example of how to use __attribute__((unused)):
void my_function(int unused_variable __attribute__((unused)))
{
    // do something
}

README
Introduction
This project covers the following topics:

How to use arguments passed to your program
Two prototypes of main and when to use them
How to use attribute((unused)) or (void) to compile functions with unused variables or parameters
Copyright and Plagiarism
Requirements
Allowed editors: vi, vim, emacs
All files will be compiled on Ubuntu 20.04 LTS using gcc, using the options -Wall -Werror -Wextra -pedantic -std=gnu89
All files should end with a new line
A README.md file, at the root of the folder of the project is mandatory
Code should use the Betty style. It will be checked using betty-style.pl and betty-doc.pl
Not allowed to use global variables
No more than 5 functions per file
Prototypes of all functions and _putchar should be included in header file called main.h
Don’t forget to push the header file
Allowed to use the standard library
How to Use Arguments Passed to Your Program
In C, arguments can be passed to your program through the command line. These arguments can be used by your program for various purposes. The main function takes two arguments: argc and argv. argc stands for argument count, and argv stands for argument vector. argc is an integer that represents the number of arguments passed to the program, including the name of the program itself. argv is an array of strings that contains the arguments passed to the program.

Here's an example of how to use arguments passed to your program:

c
Copy code
#include <stdio.h>

int main(int argc, char *argv[])
{
    int i;
    for (i = 0; i < argc; i++)
    {
        printf("arg %d: %s\n", i, argv[i]);
    }
    return 0;
}
In this example, we iterate through the argv array and print out each argument along with its index.

Two Prototypes of Main and When to Use Them
There are two prototypes for the main function:

c
Copy code
int main(void);
int main(int argc, char *argv[]);
The first prototype takes no arguments, while the second prototype takes two arguments: argc and argv.

You should use the first prototype (int main(void)) if your program does not need to accept any command-line arguments. You should use the second prototype (int main(int argc, char *argv[])) if your program needs to accept command-line arguments.

How to Use attribute((unused)) or (void) to Compile Functions with Unused Variables or Parameters
When compiling your program, you may encounter warnings about unused variables or parameters in your functions. To prevent these warnings, you can use the __attribute__((unused)) or (void) syntax.

Here's an example of how to use __attribute__((unused)):

c
Copy code
void my_function(int unused_variable __attribute__((unused)))
{
    // do something
}
In this example, we use __attribute__((unused)) to tell the compiler that the unused_variable parameter is intentionally unused.

Here's an example of how to use (void):

