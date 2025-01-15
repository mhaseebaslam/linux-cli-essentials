# LXD Commands

LXD is a modern, secure, and powerful tool that provides a unified experience for running and managing containers or virtual machines. Visit [Canonical LXD](https://canonical.com/lxd) for more information.

## Initialization

- `lxd init`: Initializes LXD before first use. This command sets up the necessary configurations and storage for LXD.

## Creating Instances

- `lxc init ubuntu:22.04 <container name>`: Creates a LXC system container with the specified name without starting it.
- `lxc launch ubuntu:24.04 <container name>`: Creates and starts a LXC system container with the specified name.
- `lxc launch ubuntu:22.04 <vm name> --vm`: Creates and starts a virtual machine with the specified name.

## Managing Instances

- `lxc list`: Lists all instances (containers and virtual machines) managed by LXD.
- `lxc info <instance>`: Shows detailed status information about the specified instance.
- `lxc start <instance>`: Starts the specified instance.
- `lxc stop <instance> [--force]`: Stops the specified instance. Use `--force` to forcefully stop it.
- `lxc delete <instance> [--force|--interactive]`: Deletes the specified instance. Use `--force` to forcefully delete it or `--interactive` for interactive confirmation.

## Accessing Instances

- `lxc exec <instance> -- <command>`: Runs a command inside the specified instance.
- `lxc exec <instance> -- bash`: Gets shell access to the specified instance (if bash is installed).
- `lxc console <instance> [flags]`: Gets console access to the specified instance.
- `lxc file pull <instance>/<instance_filepath> <local_filepath>`: Pulls a file from the specified instance to the local machine.
- `lxc file push <local_filepath> <instance>/<instance_filepath>`: Pushes a file from the local machine to the specified instance.

## Using Projects

- `lxc project create <project> [--config <option>]`: Creates a new project with the specified name and optional configuration.
- `lxc project set <project> <option>`: Configures the specified project with the given option.
- `lxc project switch <project>`: Switches to the specified project, changing the context for subsequent LXD commands.
