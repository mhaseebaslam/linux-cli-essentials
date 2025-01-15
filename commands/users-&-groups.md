# User and Group Management Commands

## User Management

- `w`: Shows which users are logged in and what they are doing. Provides information on the current system load and user activity.
- `sudo adduser <username>`: Creates a new user with the specified username. This command also sets up the user's home directory and prompts for a password.
- `sudo deluser <username>`: Deletes a user and optionally removes their home directory and mail spool.
- `sudo passwd <username>`: Sets or changes the password for a user. This command can also be used to set password policies.
- `su <username>`: Switches to the specified user. This command allows you to run commands with the privileges of another user.
- `sudo passwd -l <username>`: Locks a user account, preventing the user from logging in.
- `sudo passwd -u <username>`: Unlocks a user account, allowing the user to log in again.
- `sudo chage <username>`: Sets user password expiration date and other password aging policies. Useful for enforcing password changes at regular intervals.

## Group Management

- `id [username]`: Displays user and group IDs for the specified user. If no username is provided, it shows the IDs for the current user.
- `groups [username]`: Shows the groups a user belongs to. If no username is provided, it shows the groups for the current user.
- `sudo addgroup <groupname>`: Creates a new group with the specified name.
- `sudo delgroup <groupname>`: Deletes a group with the specified name.
