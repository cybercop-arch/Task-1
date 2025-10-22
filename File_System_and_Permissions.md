# File System Navigation & Permissions

## File System Navigation
- `pwd` — print working directory
- `ls -la` — list files with details (hidden files)
- `cd /path/to/dir` — change directory
- `cd ..` — go up one directory
- `cd ~` or `cd` — go to home directory
- `mkdir dir_name` — create directory
- `rmdir dir_name` / `rm -rf dir_name` — remove directory

## File & Directory Permissions
- `ls -l` — view permissions (rwx)
- `chmod 755 script.sh` — change permissions (owner/group/others)
- `chmod u+x script.sh` — add execute for user
- `chown user:group file` — change owner and group
- `stat file` — show detailed file info
- Numeric permission quick reference:
  - `7` = read+write+execute (rwx)
  - `6` = read+write (rw-)
  - `5` = read+execute (r-x)
  - `4` = read only (r--)
