# Linux File Permissions

## Why permissions matter

Linux uses permissions to control who can read, modify, or execute a file, and who can access a directory. Understanding permissions is important for system administration and defensive security because access should be limited to the people and processes that need it.

## The three permission types

- **Read (`r`):** allows a file to be read. For a directory, it allows the names of entries to be listed.
- **Write (`w`):** allows a file to be changed. For a directory, it allows entries to be created, removed, or renamed, subject to other permissions.
- **Execute (`x`):** allows a file to be run as a program or script. For a directory, it allows traversal through that directory.

## Who receives permissions?

Permissions are shown for three categories:

- **Owner:** the user who owns the file.
- **Group:** users who belong to the file's group.
- **Others:** everyone else.

## Reading `ls -l`

Run:

```bash
ls -l
```

A permissions field may look like this:

```text
-rw-r--r-- 1 user user 1200 Nov 6 10:00 notes.txt
```

The first character indicates the file type. The next nine characters are permission groups:

- `rw-`: owner can read and write.
- `r--`: group can read.
- `r--`: others can read.

A dash means that permission is not granted.

## Checking permissions

```bash
ls -l notes.txt
```

## Changing permissions

The `chmod` command changes permissions. For example, this gives the owner read and write access, and gives group and others read access:

```bash
chmod 644 notes.txt
```

The numeric values represent combinations of permissions: read is 4, write is 2, and execute is 1. They are added together for each category.

## Ownership

The `chown` command changes the owner or group of a file. Changing ownership usually requires appropriate privileges.

```bash
chown username:groupname notes.txt
```

Only use ownership-changing commands in a test environment where you have permission to make the change.

## Security connection

Permissions help reduce unnecessary access. A useful habit is to check who owns a file and which users can access it, rather than assuming that every file should be available to everyone.

## What I am learning

I am learning how to read the permission string shown by `ls -l`, distinguish owner, group, and other permissions, and understand why least-privilege access matters.
