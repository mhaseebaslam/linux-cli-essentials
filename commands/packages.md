# Package Management Commands

## Package Management (APT)

- `sudo apt install <package>`: Installs a package from the APT repository. Requires root privileges.
- `sudo apt install -f --reinstall <package>`: Reinstalls a broken package, fixing any missing dependencies. The `-f` option stands for "fix broken".
- `apt search <package>`: Searches for packages in the APT repository that match the specified name or description.
- `apt-cache policy <package>`: Lists available versions of a package and shows which version is currently installed and which version is available from the repository.
- `sudo apt update`: Updates the package lists from the repositories. This should be run before upgrading or installing packages to ensure you have the latest information.
- `sudo apt upgrade`: Upgrades all upgradable packages to their latest versions. This will not remove any packages.
- `sudo apt remove <package>`: Removes a package but leaves its configuration files. Useful if you plan to reinstall the package later.
- `sudo apt purge <package>`: Removes a package and all its configuration files. Useful for completely removing a package from the system.

## Package Management (Snap)

- `snap find <package>`: Searches for Snap packages that match the specified name or description.
- `sudo snap install <snap_name>`: Installs a Snap package. Requires root privileges.
- `sudo snap remove <snap_name>`: Removes a Snap package. Requires root privileges.
- `sudo snap refresh`: Updates all installed Snap packages to their latest versions.
- `snap list`: Lists all installed Snap packages along with their versions and revision numbers.
- `snap info <snap_name>`: Displays detailed information about a Snap package, including its description, publisher, and available versions.
