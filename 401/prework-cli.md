# The Command Line
*This is a summary from [Ryans Tutorials](ryanstutorials.net/linuxtutorial)*

*What is it?*
Also known as the terminal, the command line is a linux/unix text (as opposed to graphical) interface.

*How does it work and how do I get to one?*
It presents you with a prompt that accepts text commands.  If the command is valid, it is executed immediately after and any feedback is displayed in the lines following the command.

Most operating systems have an application called Terminal.

---
##### In linux there are often different ways to accomplish the same result.  This summary discusses one or a few of the common ways.
---

## Basic Navigation
Basic navigation involves getting to or referencing the correct location in the system using commands.  For example:

- `pwd`, Print Working Directory, tells you where you are now.

- `ls`, short for list, shows you the content of the relevan directory

### Paths
The linux file system is hierarchical.  The root directory, denoted by a single slash (/) is at the top of the structure and has subdirectories that typically have their own subdirectories.

A Path show how to get to a particular file or directory.  There are two kinds of paths:

- Absolute - show location relative to the root directory

- Relative - show location relative to the current directory

To build a path, you may use the following references:

- `~` (tilde) - shortcut for your home directory
- `.` (dot) - reference to the current directory
- `..` (dot dot) - reference to the parent directory

For example, to see the contents of the parent directory: `ls ../`

Us `cd [location]` to move to a different directory.  For example, to go to the home directory use `cd ~` or to go to the parent directory use `cd ..`

## Files
In linux everything is a file.
> A text file is a file, a directory is a file, your keyboard is a file (one that the system reads from only), your monitor is a file (one that the system writes to only) etc.

---
##### Linux is case sensitve - Important!
---

While spaces can be handled (using quotes or escape characters) in file and directory names, it is best practice to avoid doing so.

### Hidden files and directories
Hidden file names begin with `.` (full stop).
> Files and directories may be hidden for a variety of reasons. Configuration files for a particular user (which are normally stored in their home directory) are hidden for instance so that they don't get in the way of the user doing their everyday tasks.

To disply hidden files use `ls -a`

## Manual pages
Manual pages explain evey command available and what they do.  Invoke the manual pages with `man <coomand to look up>`

- To search the manual pages by keyword use `man -k <keyword>`

- To serch within a manual page use `/ <keyword>`

### Running commands
A command is always the first thing you type, optionally followed by arguments, which are separated by spaces.  Options are a common argument, usually entered before other arguments, that directs the behavior of the command.

Options typically start with a dash ( - ).  There are two ways to enter options:
- Short hand with one dash (-) and one letter or more than one letter if chaining options
- Long hand with two dashes (--) and a word

---
##### Keep in mind there is no undo in linux command line
---

## File manipulation
*Note all references to sources or directories are paths.*

Make directory: `mkdir [options] <directory>`.  Some commn options are:
- `-p` - make paren directories as needed
- `-v` - short for verbose (--verbose), which tells us what is doing
  - `pv` - link both of the above

Remove directory: `rmdir [options] <directory>`

Create file: `touch [options] <filename>`.  Touch modifies the access and modification times on a file, however if the file does not exist, it create it.

Copy file: `cp [options] <source> <destination>`.  Note the destination could be a path to a file or a directory.

Move file or directory: `mv [options] <source> <destination>`.  mv can be used to rename a file (same directory as present file but different filename).

Remove file: `rm [options] <file>`.  Use `rm -r <directory>` to remove a non-empty directory.

---

[Back to table of contents](../README.md)