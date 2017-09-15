# Guide to Bash (Bourne Again Shell)
A guide to simple commands in the terminal that you will be frequently using to compile
and interact with your Java programs. The guide also assumes you have a working understanding
of how directory trees work on computers (i.e. folders inside folders, etc.).

Note that for any of these commands, you can use relative paths or absolute paths.

```
ls
```
Lists out the contents of the current directory.

```
ls -a
```
Lists out all the contents of the current directory, including hidden files with a "." in front
of their name.

```
cd new_directory
```
Changes the terminal location from the current directory to a directory called "new_directory".

```
cd ..
```
Moves the terminal location up to the next directory "up" the directory tree. If my current
directory before I run this command is "C:\Program Files\Java\jdk1.8.0_144\bin", it will be
"C:\Program Files\Java\jdk1.8.0_144" after.

```
touch filename.extension
```

The touch command creates a file called "filename" with the file type extentsion "extension". For example,
if I were to type the command "touch HelloWorld.java", it would create a Java file in my current directory
called "HelloWorld.java".

```
mkdir new_directory
```
Stands for "MaKe DIRectory" and creates a new directory inside the current directory entitled "new_directory".

```
rmdir directory
```
ReMoves the DIRectory "directory" from the current working directory. "directory" must be empty to use this command.

```
rm -i file
```
ReMoves "file" from the current directory after prompting the user to type "y" to delete, or "n" to cancel deletion.
Note, I ONLY want you to use this command with the "-i" option. It's much safer that way, trust me.


# TERMS:
- Directory = A location in the computer file system, which may be empty, or contain other directories or files.
- Path = An address in the catalog of the file system.
- Absolute Path = The full path of a directory or file, i.e. "C:\Program Files\Java\jdk1.8.0_144\bin".
- Relative Path = The path of the directory relative to where the terminal is located, i.e. if I was in the directory "C:\Program Files\Java", then the directory of the JDK bin would be "jdk1.8.0_144\bin" relative to where I am.
