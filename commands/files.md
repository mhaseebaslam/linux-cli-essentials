# File Management Commands

## File Management

- `ls`: Lists files and directories in the current directory. Options like `-l` for detailed listing and `-a` for hidden files can be used.
- `touch <filename>`: Creates an empty file if it doesn't exist or updates the last accessed and modified timestamps of the file.
- `cp <source> <destination>`: Copies files or directories from the source path to the destination path. Use `-r` to copy directories recursively.
- `mv <source> <destination>`: Moves files or directories from the source path to the destination path. It can also be used to rename files or directories.
- `rm <filename>`: Deletes a file. Use `-r` to remove directories and their contents recursively.

## Directory Navigation

- `pwd`: Displays the current directory path. Useful for confirming your current location in the filesystem.
- `cd <directory>`: Changes the current directory to the specified directory. Use `cd ..` to move up one directory level.
- `mkdir <dirname>`: Creates a new directory with the specified name. Use `-p` to create parent directories as needed.

## File Permissions and Ownership

- `chmod [who][+/-][permissions] <file>`: Changes file permissions. For example, `chmod u+x <file>` makes a file executable by its owner.
- `chmod u+x <file>`: Makes a file executable by its owner. `u` stands for user, `+` adds a permission, and `x` stands for execute.
- `chown [user]:[group] <file>`: Changes the owner and group of a file. For example, `chown user:group <file>` sets the owner to `user` and the group to `group`.

## Searching and Finding

- `find [directory] -name <search_pattern>`: Finds files and directories matching the search pattern within the specified directory and its subdirectories.
- `grep <search_pattern> <file>`: Searches for a pattern within a file. Use `-r` to search recursively in directories.

## Archiving and Compression

- `tar -czvf <name.tar.gz> [files]`: Compresses files into a tar.gz archive. `-c` creates a new archive, `-z` compresses it with gzip, `-v` shows progress, and `-f` specifies the filename.
- `tar -xvf <name.tar.[gz|bz|xz]> [destination]`: Extracts a compressed tar archive. `-x` extracts files, `-v` shows progress, and `-f` specifies the filename. The destination is optional.

## Text Editing and Processing

- `nano [file]`: Opens a file in the Nano text editor. Useful for quick and simple text editing.
- `cat <file>`: Displays the contents of a file. Can be used to concatenate multiple files and display their content.
- `less <file>`: Displays the paginated content of a file. Allows for easy navigation through large files.
- `head <file>`: Shows the first few lines of a file. Use `-n` to specify the number of lines.
- `tail <file>`: Shows the last few lines of a file. Use `-n` to specify the number of lines.
- `awk ‘{print}’ [file]`: Prints every line in a file. Can be used for more complex text processing and data extraction.
