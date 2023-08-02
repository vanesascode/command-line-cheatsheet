# Command line cheatsheet

In command-line interfaces, a command usually consists of a utility, flags, and arguments. Here's a breakdown of each component: 
 
**1. Utility:** The utility is the main executable or program that performs a specific task or operation. It is the command you run to execute a particular action. Examples of utilities include "ls" for listing files, "mkdir" for creating directories, or "ping" for testing network connectivity. 
 
**2. Flags/Options:** Flags, also known as options, modify the behavior of the utility. They are typically preceded by a hyphen (-) or double hyphen (--). Flags can enable/disable certain features, provide additional information, or change the default behavior of the utility. For example, the "-l" flag in the "ls" command is used to display detailed file information, while the "--recursive" flag in the "cp" command is used to copy directories and their contents recursively. 
 
**3. Arguments:** Arguments are the inputs or parameters passed to the utility to specify the specific files, directories, or settings to be used. They provide the necessary information for the utility to perform its intended task. Arguments are typically provided after the utility and any flags. For example, in the command "mkdir -p new_directory", "new_directory" is the argument specifying the name of the directory to be created. 
 
It's important to note that the usage of utilities, flags, and arguments can vary depending on the specific command-line interface, operating system, or utility being used.


## 🌈GO

### 🔷 To go to the next directory (e.g. newfolder) in the file system:

In windows: 

`cd newfolder`

In Unix-like systems (Linux, macOS, BSD):

`cd newfolder`

### 🔷 To go to the previous directory (e.g. previousfolder) in the file system:

In windows: 
`cd..`

In Unix-like systems (Linux, macOS, BSD):

`cd ..`

***

## 🌈PRINT

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

`ls`

### 🔷 To list the names of all folders and files in a particular folder and in a detailed way:

In windows: 

`dir C:\Users /a`

The "/a" option is used to display hidden files.

In Unix-like systems (Linux, macOS, BSD):

`ls -l C:\Users`

-l: It specifies that the command should produce a long listing format. In this format, each file or directory is displayed on a separate line with detailed information such as file permissions, ownership, size, and modification date.

***

### 🔷 To list the names of all files (only) in the current directory, one file per line:

In Windows: 

`dir /b /a-d`

The "/b" option is used to show only the bare file names without any additional information. The "/a-d" option is used to exclude directories from the listing, ensuring that only file names are shown. 

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

## 🌈CLEAR

In windows: 
`cls`

In Unix-like systems (Linux, macOS, BSD):
`clear`

***

## 🌈CREATE

### 🔷 To create an empty file named (e.g. "newfile.txt") in the current working directory:

In windows: 

`echo. > newfile.txt`
or
`cd > newfile.txt`

The "echo" command redirects an empty string ("-n" prevents a newline character) to the specified file, effectively creating an empty file: 

In Unix-like systems (Linux, macOS, BSD):

`cat > newfile.txt`

*** 
### 🔷 To create a directory (e.g. files) inside another directory (e.g. tmp) that doesn't exist either: 

In windows: 

`mkdir tmp\files`

In Unix-like systems (Linux, macOS, BSD):

`mkdir tmp/files` or `mkdir tmp\files`

***

## 🌈COPY

### 🔷To copy a file (e.g. newfile.txt) into a directory (e.g. tmp/files/):

In windows: 

`copy newfile.txt tmp\files\`

In Unix-like systems (Linux, macOS, BSD):

`cp newfile.txt tmp\files\`

*** 

## 🌈MOVE

### 🔷To move a file (e.g. newfile.txt) into a directory (e.g. tmp):

In windows: 

`move newfile.txt tmp`

In Unix-like systems (Linux, macOS, BSD):

`mv newfile.txt tmp`

***

## 🌈OPEN

### 🔷To open a file (e.g. filename.txt) from the command prompt:

In windows: 

`start filename.txt`

In macOS: 

`open filename.txt`

Int Linux: 

`xdg-open filename.txt`

***

## 🌈FIND

### 🔷To find all files containing the exact name (e.g. music) that is inside the root folder. 

In windows: 

`dir /s /b *music*`

- "/s" is an option that makes the command search for files in the current directory and all its subdirectories. 
- "/b" is another option that displays only the file names without any additional information. 
- "**" is a pattern that filters the results to include only files whose name includes that word. 

In Unix-like systems (Linux, macOS, BSD):

`find / -name music`

### 🔷To find all files containing an extension (e.g. "mp3") within the current directory and its parent.

In windows: 

`dir /s /b *.mp3`

- "/s" is an option that makes the command search for files in the current directory and all its subdirectories. 
- "/b" is another option that displays only the file names without any additional information. 
- "*.mp3" is a pattern that filters the results to include only files with the ".mp3" extension. 

In Unix-like systems (Linux, macOS, BSD):

`find . -name *.mp3`

 - "." represents the current directory. You can replace it with a specific directory path if you want to search in a different location. 
 - "-name" is an option that specifies the search criteria based on the file name. 
 - "*.mp3" is a pattern that filters the results to include only files with the ".mp3" extension.

### 🔷To print the lines that contain a word (e.g. music) in a particular file (e.g. music.txt):

In windows: 

`type music.txt | findstr "music"`

In Unix-like systems (Linux, macOS, BSD):

`cat music.txt | grep music`

***

## 🌈REMOVE
Please note that deleting files is a permanent action, and once a file is deleted, it cannot be easily recovered. Exercise caution when using these commands.

### 🔷To remove a file (e.g. newfile.txt) in the current folder:

In windows: 

`del newfile.txt`

or: 

`erase filename.txt`

In Unix-like systems (Linux, macOS, BSD):

`rm newfile.txt`

***

### 🔷To remove several files (e.g. one.txt and two.txt) at the same time: 

In windows:  

`del one.txt two.txt`

In Unix-like systems (Linux, macOS, BSD):

`rm one.txt two.txt`

***

### 🔷To delete all the files and sub-directories recursively within a directory (e.g. files, and you are in the previous directory to it):

In windows: 

`rmdir /s files`

When you run the "rmdir /s" command followed by the directory name, it will delete the directory and all of its contents.

In Unix-like systems (Linux, macOS, BSD):

`rm -r files` 

When you run the "rm -r" command followed by the directory name, it will delete the directory and everything inside it, including all files and subdirectories.

***

👉 If you have files starting with a dot (hidden files) in the directory you want to delete, you can modify the command accordingly:

🔻**Warning**🔻: The following commands are extremely dangerous and can potentially delete important files or directories. It is highly recommended not to run this command unless you fully understand its implications. 

In windows: 

`del /s /q *`

- "/q" is an option that suppresses the confirmation prompt, meaning it won't ask for confirmation before deleting each file. 
- "*" is a wildcard character that matches any file name in the current directory. 
- ".*" is another wildcard that matches any hidden files in the current directory. 

In Unix-like systems (Linux, macOS, BSD):

`rm -rf * .*`

Explanation: 
- "rm" is the command used to remove or delete files and directories. 
- "-rf" are options used with the "rm" command. "r" stands for recursive, allowing deletion of directories and their contents. "f" stands for force, which means no confirmation prompt will be given before deleting. 
- "*" is a wildcard character that matches any file or directory name in the current directory. 
- ".*" matches hidden files and directories in the current directory. 
 
Combining these elements, the command "rm -rf * .*" attempts to delete all files and directories, including hidden ones, in the current directory. 

***

### 🔷To remove a directory (e.g. files). You have to be at least in the previous directory of the file system in order to do it:

In windows: 

`rmdir files`

In Unix-like systems (Linux, macOS, BSD):

`rmdir files`

***

## 🌈SYSTEM MANAGEMENT

### 🔷To view running processes:

In windows: 

`tasklist`

In macOS/Linux: 

`ps`

***

### 🔷To terminate processes: 

In windows: 

`taskkill`

For instance, if you want to terminate a process called "notepad.exe," the command would be:

`taskkill /F /IM notepad.exe`

The "/F" flag is used to forcefully terminate the process, and the "/IM" flag is used to specify the image name (process name). 

In macOS/Linux: 

`kill`

***

## 🌈NETWORK-RELATED-TASKS

### 🔷To check network connectivity: 

`ping`

### 🔷To view network configurations (and see your IP Address, for example): 

In windows: 

`ipconf`

In macOS/Linux: 

`ifconfig`

### 🔷To display network statistics: 

`netstat`

***

## 🌈TIPS 

- To cancel a command that is being executed, press `ctrl + c`
- To autocomplete a file or folder name, use the `tab key`.
- To repeat any command you have used in the past, use the `up arrow`, and it will show you each command, one by one.

