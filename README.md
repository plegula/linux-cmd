# linux-cmd
## Kill by name
```bash
ps -ef | grep '[process_part_name]' | grep -v grep | awk '{print $2}' | xargs -r kill -9
```
## Connect to Wi-Fi
```bash
nmcli device wifi connect "NAZWA_SIECI" password "HASŁO"
```
