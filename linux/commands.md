# Linux commands - My notes

## Navigation

- 'pwd' - displays the current directory.
- 'ls' - lists files and directories.
- 'ls -la' - lists files, including hidden files.
- 'cd folder' - moves into a directory.
- 'cd ..' - moves to the parent directory.
- 'cd ~' - moves to the home directory.

## File and deployment

- 'mkdir name' - creates a directory.
- 'touch file.txt' - creates an empty file if it does not exist.
- 'cat file.txt' - displays content of a file.
- 'cp source.txt destination.txt' - copies a file.
- 'cp file.txt directory/' - copies a file into a directory.
- 'mv old.txt new.txt' - renames or moves a file.
- 'mv file.txt directory/' - moves a file into a directory.
- 'rm file.txt' - deletes a file.
- 'ls -l' - displays file with permissions,ownership, size, and modification time.
- 'ls -ld directory' - displays information about the directory itself.


## File Search

- 'find . -type f -name "*.txt" - finds all files ending in .txt under the current directory.
- 'find . -type f -name "commands.md" - finds files named commands.md.

## File Permissions

- 'ls -l file.txt' - displays file permissions and ownership.
- 'chmod u+x file.sh' - adds execute permission for the owner.
- 'chmod u-x file.sh' - removes execute permission for the owner.
- 'chmod 644 file.txt' - owner can read and write; group and others can read.
- 'chmod 755 file.txt' - owner can read, wirte, and execute; groups and others can read and execute.
- 'chmod 700 directory' - owner has full permissions; group and others have no permissions.

Permission values:
- r = 4 (read);
- w = 2 (write);
- x = 1 (execute).

## Processes 

- 'ps' - displays processes associated with the current terminal.
- 'ps aux' - displays a broader list of running processes.
- 'top' - monitors processes and resource usage interactively; press q to quit.
- 'sleep 300 &' - starts a test process in the background.
- 'jobs' - lists jobs managed by the current shell.
- 'ps aux | grep '[s]leep'' - searches for the test process.
- 'kill "PID"' - sends the default termination signal to the specified process.

## Services

- 'systemctl status ssh' - displays the status of the SSH service.
- 'systemctl is-active ssh' - checks whether the service is currently active.
- 'systemctl is-enabled ssh' - checks whether the service is enabled for the usual automatic startup mechanism.
- 'systemctl status ssh.socket' - displays the status of the SSH rocket unit.
