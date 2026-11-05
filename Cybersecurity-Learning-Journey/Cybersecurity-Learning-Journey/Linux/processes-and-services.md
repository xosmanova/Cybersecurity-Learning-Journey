# Linux Processes and Services

## What is a process?

A process is a running instance of a program. The operating system assigns each process a process ID (PID).

## Useful commands

### `ps`

Displays process information.

```bash
ps
ps aux
```

`ps aux` displays a broader list of processes on many Linux distributions.

### `top`

Shows a live, updating view of processes and system resource use.

```bash
top
```

Press `q` to exit.

### `uptime`

Shows how long the system has been running, along with load information.

```bash
uptime
```

## What is a service?

A service is a background program that provides a function, such as logging, networking, or remote access. On many Ubuntu systems, services are managed by `systemd`.

### `systemctl`

Can be used to inspect services.

```bash
systemctl list-units --type=service
```

To check one service:

```bash
systemctl status SERVICE_NAME
```

Replace `SERVICE_NAME` with a service that exists on your own system.

## Security connection

Knowing which processes and services are running helps with understanding normal system activity. If something looks unfamiliar, it should be investigated carefully using trusted system information and an authorised environment. A process name alone is not enough to decide that something is malicious.

## What I am learning

I am learning the difference between a process and a service, how to view running processes, and how to inspect service status on a Linux system.
