# Linux Basic Commands

## Introduction

The Linux command line is used to interact with the operating system by entering commands in a terminal. It is useful for navigating files, checking system information, and managing a computer.

The examples below are intended for a normal Ubuntu learning environment. Some commands may behave differently depending on the distribution and installed software.

## 1. Navigation

### `pwd`

Prints the path of the current working directory.

```bash
pwd
```

### `ls`

Lists files and directories in the current directory.

```bash
ls
ls -la
```

The `-l` option shows a detailed list, while `-a` also includes hidden entries.

### `cd`

Changes the current directory.

```bash
cd Documents
cd ..
cd ~
```

`..` means the parent directory, and `~` refers to the current user's home directory.

## 2. Working with files and directories

### `mkdir`

Creates a directory.

```bash
mkdir linux-notes
```

### `touch`

Creates an empty file if it does not already exist.

```bash
touch notes.txt
```

### `cp`

Copies a file.

```bash
cp notes.txt notes-backup.txt
```

### `mv`

Moves a file or changes its name.

```bash
mv notes.txt linux-notes.txt
```

### `find`

Searches for files and directories in a specified location.

```bash
find . -name "*.txt"
```

This example searches below the current directory for files ending in `.txt`.

## 3. Reading and searching text

### `cat`

Prints a file's contents.

```bash
cat notes.txt
```

### `less`

Opens a file for page-by-page reading.

```bash
less notes.txt
```

Press `q` to leave `less`.

### `grep`

Searches text for a word or pattern.

```bash
grep "error" application.log
```

This can be useful when reviewing text-based log files.

## 4. Basic system information

### `whoami`

Shows the current username.

```bash
whoami
```

### `id`

Shows the current user's user ID and group memberships.

```bash
id
```

### `uname`

Displays information about the operating system kernel.

```bash
uname -a
```

### `man`

Opens the manual page for a command.

```bash
man ls
```

## What I am learning

These commands help me move around the filesystem, read files, search text, and check basic system information. I want to become comfortable with these everyday tasks before moving on to more detailed Linux administration and log analysis.

## Practice note

When practising, I use a folder of my own notes and test files. I avoid experimenting with commands that change system-wide settings unless I understand their effect.
