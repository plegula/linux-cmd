# linux-cmd
## Kill by name
```bash
ps -ef | grep '[process_part_name]' | grep -v grep | awk '{print $2}' | xargs -r kill -9
```
## Connect to Wi-Fi
```bash
nmcli device wifi connect "NAZWA_SIECI" password "HASŁO"
```
## Show disk usage
```bash
df -h
```
## Find files by name
```bash
find /path -name "filename"
```
## Follow file output
```bash
tail -f /path/to/file
```
## Search text in files
```bash
grep -R "pattern" /path
```
## Monitor system processes
```bash
top
```

## Show inode usage
```bash
# Display inode usage for each filesystem
df -i
```

## Show local filesystem usage
```bash
# Limit output to local filesystems
df -l
```

## Search for running process
```bash
# Find a running process by name
ps aux | grep "some process name"
```

## Start interactive root shell
```bash
# Open a root shell
sudo -i
```

## Change your password
```bash
# Update your own user password
passwd
```

## Change another user's password
```bash
# Set password for a specific user
sudo passwd username
```

## Find largest files
```bash
# List top 10 largest files under /path
find /path -type f -exec du -h {} + | sort -rh | head -n 10
```

## Turn off swap usage
```bash
# Disable all swap
sudo swapoff -a
```

## Monitor process network usage
```bash
# Track network usage for a specific process (replace PID)
sudo nethogs -p PID
```
