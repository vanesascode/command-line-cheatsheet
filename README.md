# Command line cheatsheet

In command-line interfaces, a command usually consists of a utility, flags, and arguments. Here's a breakdown of each component: 
 
🔷 **1. Utility:** The utility is the main executable or program that performs a specific task or operation. It is the command you run to execute a particular action. Examples of utilities include "ls" for listing files, "mkdir" for creating directories, or "ping" for testing network connectivity. 
 
🔷 **2. Flags/Options:** Flags, also known as options, modify the behavior of the utility. They are typically preceded by a hyphen (-) or double hyphen (--). Flags can enable/disable certain features, provide additional information, or change the default behavior of the utility. For example, the "-l" flag in the "ls" command is used to display detailed file information, while the "--recursive" flag in the "cp" command is used to copy directories and their contents recursively. 
 
🔷 **3. Arguments:** Arguments are the inputs or parameters passed to the utility to specify the specific files, directories, or settings to be used. They provide the necessary information for the utility to perform its intended task. Arguments are typically provided after the utility and any flags. For example, in the command "mkdir -p new_directory", "new_directory" is the argument specifying the name of the directory to be created. 
 
It's important to note that the usage of utilities, flags, and arguments can vary depending on the specific command-line interface, operating system, or utility being used.

***

## 🌈HELP

### 🔷 To get info about a utility (e.g. dir or ls) in the same terminal: 

In windows: 

`dir /?`

In Unix-like systems (Linux, macOS, BSD):

`ls --help`

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

and more levels: 

`cd ../../../ etc.`

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

### 🔷 To list all the files that are javascript files: 

`ls *.js`

***

### 🔷 To view the current value of the environment variable $PATH:

In windows: 

`echo %PATH%`

In Unix-like systems (Linux, macOS, BSD):

`echo $PATH`

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

`mkdir tmp/files`

***

## 🌈COPY

### 🔷To copy a file (e.g. newfile.txt) into a directory (e.g. tmp/files/):

In windows: 

`copy newfile.txt tmp\files\`

In Unix-like systems (Linux, macOS, BSD):

`cp newfile.txt tmp/files/`

(if the folder "files" doesn't exist inside the supposed folder "tmp", it will create a file called "files"...)

*** 

### 🔷To copy a file (e.g. newfile) in the previous folder: 

In Unix-like systems (Linux, macOS, BSD):

`cp newfile.txt ../`

***

### 🔷To copy a file (e.g. newfile.txt) in the following folder (e.g. files) and put it a name (e.g. hello.txt): 

In Unix-like systems (Linux, macOS, BSD):

`cp newfile.txt files/hello.txt`

***

## 🌈MOVE

### 🔷To move a file (e.g. newfile.txt) into a directory (e.g. tmp) when inside the directory you have the file:

In windows: 

`move newfile.txt tmp`

In Unix-like systems (Linux, macOS, BSD):

`mv newfile.txt tmp`

### 🔷To move a file (e.g. newfile.txt) into another directory (e.g. from documents to files) without it being necessary to be inside the directory you have the file:

In Unix-like systems (Linux, macOS, BSD):

`mv /home/user/documents/newfile.txt /home/user/files/`

***

### 🔷To move a file (e.g. file.txt) into another directory (e.g. from documents to files) without it being necessary to be inside the directory you have the file, and to rename the file (e.g. newfile):

In Unix-like systems (Linux, macOS, BSD):

`mv /home/user1/documents/file.txt /home/user1/files/newfile.txt`

***

## 🌈SORT

### 🔷To sort the contents of a text file in alphabetical order.

In windows: 

`sort data.txt` 

In Unix-like systems (Linux, macOS, BSD):

`sort data.txt` 

***

## 🌈OPEN

### 🔷To open a file (e.g. filename.txt) from the command prompt:

In windows:

`start filename.txt`

***

## 🌈FIND

### 🔷To find all files containing a particular word in its title (e.g. music) and that is inside the root folder. 

In windows: 

`dir *music*`

`dir /s /b *music*`
- "/s" is an option that makes the command search for files in the current directory and all its subdirectories. 
- "/b" is another option that displays only the file names without any additional information. 

In Unix-like systems (Linux, macOS, BSD):

`ls *music*`

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

`findstr "music" music.txt`

or: 

`type music.txt | findstr "music"`

In Unix-like systems (Linux, macOS, BSD):

`grep music music.txt`

or:

`cat music.txt | grep music`

***


### 🔷To print the relative file paths, one path per line for all filenames that CONTAIN with a particular word (e.g."newfile") in the current directory:

In windows: 

`for /R %I in (*) do @echo %~dpnI | findstr /i "newfile"`

In Unix-like systems (Linux, macOS, BSD):

`grep -l newfile*`

- grep: The grep command is used to search for text patterns within files.

- -l: This option, when used with grep, instructs it to only display the names of the files that contain the pattern, rather than the specific lines where the pattern is found.

- `*` is a wildcard that matches any file in the current directory. By using *, you are telling grep to search for the pattern "newfile" in all files within the current directory.

***
  
### 🔷To print the relative file paths, one path per line for all filenames that STARTS with a particular word (e.g."newfile") in the current directory:

In windows: 

`for %I in (newfile*) do @echo %~nxI`

In Unix-like systems (Linux, macOS, BSD):

`ls newfile*`

***

### 🔷 To print all matching lines (without the filename or the file path) in all files under the current directory that CONTAIN a particular string (e.g. word)


In Unix-like systems (Linux, macOS, BSD):

`grep -r -h "word"`

-r stands for "recursive", which means that grep will search for the pattern in all files and directories within the current directory and its subdirectories.

-h stands for "no-filename", which means that grep will only print the matching lines without showing the file names.

***

### 🔷 To print all matching lines (only the filename) in all files under the current directory that CONTAIN a particular string (e.g. word)

In windows: 

`findstr /s /i /m "word" *`

***

### 🔷 To print all matching lines (with the filename) in all files under the current directory that CONTAIN a particular string (e.g. word) and the line in which it appears. 

In windows: 

`findstr /s /n "word" *`

- /s is used to search for the pattern in all files and directories within the current directory and its subdirectories.
- /n is used to display the line numbers along with the matching lines.
- "word" specifies the pattern or word you want to search for.
- `*` specifies that the search should be performed on all files.
 
In Unix-like systems (Linux, macOS, BSD):
 
`grep -r -n "word" *`

- -r stands for "recursive", which means that grep will search for the pattern in all files and directories within the current directory and its subdirectories.
- -n stands for "line number", which means that grep will display the line numbers along with the matching lines.
- "word" specifies the pattern or word you want to search for.
- `*` specifies that the search should be performed on all files.
 
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

or try:

`rmdir -r files`

When you run the "rmdir /s" command followed by the directory name, it will delete the directory and all of its contents.

In Unix-like systems (Linux, macOS, BSD):

`rm -r files` 

When you run the "rm -r" command followed by the directory name, it will delete the directory and everything inside it, including all files and subdirectories.

***

👉 If you have files starting with a dot (hidden files) in the directory you want to delete, you can modify the command accordingly:

🔻**Warning**🔻: The following commands are extremely dangerous and can potentially delete important files or directories. It is highly recommended not to run this command unless you fully understand its implications. 

In windows: 

`del /s /q /a:h *`

- "/q" is an option that suppresses the confirmation prompt, meaning it won't ask for confirmation before deleting each file. 
- `*` is a wildcard character that matches any file name in the current directory. 
- `/a:h` This option specifies that the deletion should include hidden files.  

In Unix-like systems (Linux, macOS, BSD):

`rm -rf * .*`

Explanation: 
- "rm" is the command used to remove or delete files and directories. 
- "-rf" are options used with the "rm" command. "r" stands for recursive, allowing deletion of directories and their contents. "f" stands for force, which means no confirmation prompt will be given before deleting. 
- `*` is a wildcard character that matches any file or directory name in the current directory. 
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

### 🔷To display the kernel name:

`uname`

It stands for "Unix Name" and is typically used on Unix-like systems such as Linux or macOS.

With `-a` it displays all available information about the system, including the kernel name, network node hostname, kernel release, kernel version, machine hardware name, processor type, hardware platform, and operating system.

In windows: 

`systeminfo` 

In windows it provides detailed information about the operating system and hardware configuration of a Windows system. It will display various system information such as the operating system name, version, build number, system manufacturer, system model, processor information, installed physical memory (RAM), and more.

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

`taskkill /f /im notepad.exe`

The "/f" flag is used to forcefully terminate the process, and the "/im" flag is used to specify the image name (process name). 

In macOS/Linux: 

`killall -9 notepad`

-9: This option specifies the signal to send. In this case, -9 sends the SIGKILL signal, which forcefully terminates the process.

***

## 🌈NETWORK-RELATED-TASKS

### 🔷To check network connectivity: 

`ping`

### 🔷To view network configurations (and see your IP Address, for example): 

In windows: 

`ipconfig`

In macOS/Linux: 

`ifconfig`

### 🔷To display network statistics: 

`netstat`

***

## 🌈TIPS 

- To cancel a command that is being executed, press `ctrl + c`
- To autocomplete a file or folder name, use the `tab key`.
- To repeat any command you have used in the past, use the `up arrow`, and it will show you each command, one by one.

## 🌈SYMBOLS (in Linux)

### 🔷; (semicolon):

The `;` allows you to run multiple commands sequentially, regardless of the success or failure of the preceding command.

For example:

`command1 ; command2`

In this case, command1 will run first, and then command2 will run regardless of the exit status of command1.

### 🔷, (comma):

The `,` is similar to ; in that it allows you to run multiple commands sequentially. However, unlike ;, the exit status of the preceding command is significant.

For example:

`command1 , command2`

In this case, command1 will run first, and then command2 will run only if command1 succeeds (i.e., returns an exit status of 0).

### 🔷&& (double ampersand):

The `&&`  allows you to run multiple commands sequentially, but only if the preceding command succeeds (returns an exit status of 0).

For example:

`command1 && command2`

In this case, command1 will run first, and if it succeeds, command2 will run. If command1 fails, command2 will not be executed.

### 🔷| (pipe):

The `|` is used to redirect the output of one command as input to another command (known as "piping").

For example:

`command1 | command2`

In this case, the output of command1 is passed as input to command2. This is useful for chaining commands together and processing data in a pipeline.

### 🔷|| (double pipe):

The `||` allows you to run multiple commands sequentially, but only if the preceding command fails (returns a non-zero exit status).

For example: 

`command1 || command2` 

In this case, command1 will run first, and if it fails, command2 will run. If command1 succeeds, command2 will not be executed.


