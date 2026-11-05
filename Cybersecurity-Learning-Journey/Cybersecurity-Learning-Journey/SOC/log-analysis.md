# Introduction to Log Analysis

## What is a log?

A log is a record of events produced by an operating system, application, or network device. Logs can help administrators understand what happened and help security analysts investigate unusual activity.

## Examples of events recorded in logs

- Successful or failed sign-in events.
- Application errors.
- Service start and stop events.
- Changes to system configuration.
- Network connection information, where logging is enabled.

## Useful log fields

A log entry may contain:

- Timestamp: when the event was recorded.
- Host or device: where it occurred.
- User or account: which identity was involved, if known.
- Event type or ID: what kind of event was recorded.
- Source address: where a network request came from, if available.
- Result or status: whether an action succeeded or failed.

Not every log contains all these fields.

## Viewing logs on Ubuntu

On systems that use systemd, `journalctl` can be used to view the system journal.

```bash
journalctl
```

Show a limited number of recent entries:

```bash
journalctl -n 20
```

Show entries from the current boot:

```bash
journalctl -b
```

Inspect the status of a service:

```bash
systemctl status SERVICE_NAME
```

Replace `SERVICE_NAME` with a real service on the system. The available services depend on the installation.

## A simple review approach

When reviewing a log entry, ask:

1. When did the event happen?
2. Which system recorded it?
3. Which user or process was involved?
4. What action or result was recorded?
5. Is there related activity before or after this event?
6. What additional evidence would be needed before drawing a conclusion?

## Important point

One failed login or one unusual event does not automatically prove an attack. Analysts need context, related events, and reliable evidence before classifying activity.

## What I am learning

I am learning what logs contain, how to view basic Ubuntu system logs, and why timestamps and context matter when reviewing events.
