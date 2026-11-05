# Linux Users and Groups

## Introduction

Linux supports multiple user accounts. Groups make it easier to manage permissions for several users who need similar access.

Understanding users and groups is useful when reviewing who can access a system and its files.

## Useful commands

### `whoami`

Shows the username of the current session.

```bash
whoami
```

### `id`

Shows the user ID (UID), primary group ID (GID), and supplementary groups.

```bash
id
```

### `groups`

Lists the groups associated with a user.

```bash
groups
```

### `who`

Shows users currently logged in, where supported by the system's session setup.

```bash
who
```

### `getent passwd`

Displays account entries from the system's configured account databases.

```bash
getent passwd
```

The output contains account information such as username and home directory. It does not display users' plain-text passwords.

## Users, groups, UID, and GID

- A **user account** represents an identity used to access the system.
- A **group** is a collection of users used for permission management.
- A **UID** is a numeric user identifier.
- A **GID** is a numeric group identifier.

## Security connection

Reviewing accounts and group memberships can help an administrator notice accounts that are no longer needed or permissions that are broader than necessary. Changes should follow the organisation's approval process.

## What I am learning

I am learning how Linux identifies users and groups and how group membership can affect access to files and system resources.
