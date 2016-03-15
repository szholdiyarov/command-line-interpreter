# A simple commmand line interpreter(unix shell) using c

A unix command line interpreter using C allowing the user to type commands. Like all unix shells, it supports filename, wildcarding, piping, here documents, command substitution, variables and control structures for condition testing and iteration. 

The application runs using GCC compiler. The command entered by the user is processed first. If the user input is blank, it will be reported and command will be read again from the input buffer. For a non-blank input, the command will be broken into tokens separated by the delimiter space. This is achieved by the in built c function strtok()

Then a child is created using the fork command. Now, the current process is replace by the command entered by the user. If the command's executable binary is found, the command is executed, otherwise the error message is printed.



