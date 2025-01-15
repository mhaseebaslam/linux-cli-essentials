# System Commands

## System Information

- `uname -a`: Displays all system information, including the kernel name, version, and other details.
- `hostnamectl`: Shows current hostname and related details such as the operating system, kernel version, and architecture.
- `lscpu`: Lists detailed CPU architecture information, including the number of CPUs, threads, cores, sockets, and more.
- `timedatectl status`: Shows the current system time, time zone, and synchronization status.

## System Monitoring and Management

- `top`: Displays real-time system processes, including CPU and memory usage. Useful for monitoring system performance.
- `htop`: An interactive process viewer (needs installation). Provides a more user-friendly interface compared to `top`, with additional features like process tree view.
- `df -h`: Shows disk usage in a human-readable format. Displays the amount of disk space used and available on all mounted filesystems.
- `free -m`: Displays free and used memory in MB. Provides an overview of the system's memory usage, including total, used, free, shared, buffer/cache, and available memory.
- `kill <process id>`: Terminates a process by its process ID (PID). Useful for stopping unresponsive or unwanted processes.

## Running Commands

- `[command] &`: Runs a command in the background, allowing you to continue using the terminal while the command executes.
- `jobs`: Displays background commands that are currently running or stopped. Useful for managing multiple background tasks.
- `fg <command number>`: Brings a background command to the foreground, allowing you to interact with it directly.

## Service Management

- `sudo systemctl start <service>`: Starts a service. Useful for initiating services that are not running.
- `sudo systemctl stop <service>`: Stops a service. Useful for stopping services that are running.
- `sudo systemctl status <service>`: Checks the status of a service, providing information on whether it is active, inactive, or failed.
- `sudo systemctl reload <service>`: Reloads a service’s configuration without interrupting its operation. Useful for applying configuration changes without restarting the service.
- `journalctl -f`: Follows the journal, showing new log messages in real time. Useful for monitoring system logs as they are generated.
- `journalctl -u <unit_name>`: Displays logs for a specific systemd unit. Useful for troubleshooting and monitoring specific services.

## Cron Jobs and Scheduling

- `crontab -e`: Edits cron jobs for the current user. Opens the user's crontab file in the default text editor, allowing you to schedule tasks.
- `crontab -l`: Lists cron jobs for the current user. Displays the contents of the user's crontab file, showing all scheduled tasks.
