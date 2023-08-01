# Command line cheatsheet

In command-line interfaces, a command usually consists of a utility, flags, and arguments. Here's a breakdown of each component: 
 
**1. Utility:** The utility is the main executable or program that performs a specific task or operation. It is the command you run to execute a particular action. Examples of utilities include "ls" for listing files, "mkdir" for creating directories, or "ping" for testing network connectivity. 
 
**2. Flags/Options:** Flags, also known as options, modify the behavior of the utility. They are typically preceded by a hyphen (-) or double hyphen (--). Flags can enable/disable certain features, provide additional information, or change the default behavior of the utility. For example, the "-l" flag in the "ls" command is used to display detailed file information, while the "--recursive" flag in the "cp" command is used to copy directories and their contents recursively. 
 
**3. Arguments:** Arguments are the inputs or parameters passed to the utility to specify the specific files, directories, or settings to be used. They provide the necessary information for the utility to perform its intended task. Arguments are typically provided after the utility and any flags. For example, in the command "mkdir -p new_directory", "new_directory" is the argument specifying the name of the directory to be created. 
 
It's important to note that the usage of utilities, flags, and arguments can vary depending on the specific command-line interface, operating system, or utility being used.

## PRINT

### 🔷 To print what you write in the command line:

`echo hello world`

***

### 🔷 To print the current working directory:

In Windows: 

`cd`

In Unix-like systems (Linux, macOS, BSD):

`pwd`

***

### 🔷 To list the names of all folders and files in the current directory:

In windows: 

`dir`

In Unix-like systems (Linux, macOS, BSD):

`ls -1`

The "-1" option ensures that each file is listed on its own line for better readability.

***

### 🔷 To list the names of all files (only) in the current directory, one file per line:

In Windows: 

`dir /B /A-D`

The "/B" option is used to show only the bare file names without any additional information. The "/A-D" option is used to exclude directories from the listing, ensuring that only file names are shown. 

***

### 🔷 To print the contents of a file (e.g. "newfile.txt") in the current directory:

In windows: 

`type newfile.txt`

In Unix-like systems (Linux, macOS, BSD):

`cat newfile.text`

'cat' is short for "concatenate" and is primarily used to display the contents of one or more files. However, it can also be used to create, combine, or manipulate files.

***
 
### 🔷 To print the last lines (e.g. 5) of a file (e.g. "newfile.txt"):

In Unix-like systems (Linux, macOS, BSD):

`tail -n 5 newfile.txt`

"tail" command displays the last part of a file or a stream of data. By default, it shows the last 10 lines.
The "-n" option is used to specify the number of lines to be shown, in this case, 5.

***

## CREATE

### 🔷 To create an empty file named (e.g. "newfile.txt") in the current working directory:

In windows: 

`echo. > newfile.txt`

The "echo" command redirects an empty string ("-n" prevents a newline character) to the specified file, effectively creating an empty file: 

In Unix-like systems (Linux, macOS, BSD):

`touch newfile.txt`

*** 
### 🔷 To create a directory (e.g. files) inside another directory (e.g. tmp) that doesn't exist either: 

In windows: 

`mkdir tmp\files`

In Unix-like systems (Linux, macOS, BSD):

`mkdir -p tmp/files`

The "-p" option is used to create parent directories if they don't exist. This ensures that both the "tmp" directory and the "files" directory are created if they are not already present in the current working directory.

## COPY

### 🔷To copy a file (e.g. newfile.txt) into a directory (e.g. tmp/files/):

In windows: 

`copy newfile.txt tmp\files\`

In Unix-like systems (Linux, macOS, BSD):

`cp newfile.txt tmp/files/`

*** 

## MOVE

### 🔷To copy a file (e.g. newfile.txt) into a directory (e.g. tmp):

In windows: 

`move newfile.txt tmp`

In Unix-like systems (Linux, macOS, BSD):

`mv newfile.txt tmp`

