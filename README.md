# linux-cmd
#Kill by name
ps -ef | grep '[process_part_name]' | grep -v grep | awk '{print $2}' | xargs -r kill -9

#Connect to Wi-Fi
nmcli device wifi connect "NAZWA_SIECI" password "HASŁO"
