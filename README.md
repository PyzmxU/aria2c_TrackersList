# Quick Start

```
bash aria2c_TrackersList/go.sh
```

# aria2c rule
This is an instration about how to configure the enviroment about downloading torrent.

1.The configure file is `$HOME/.aria2/aria2.conf`

2.Search the project which have saved many TrackerLists Files
`https://github.com/ngosang/trackerslist`

3.In `aria2.conf` , You only need to add a line:
```
bt-tracker=<URI>,<URI>,<URI>,<URI>,<URI>....
```

# Aria2c script


1.We advise you locate this script in `/usr/lib`

2.If you have this ability,I advise you to add it to __crontab__

# Crontab Configuration

1.Check the Time of the server
```
date
```

2.Select the editor of the __crontab__

```
select-editor
```

3.use __crontab__

Look at crontab:
```
crontab -l
```
Add task to crontab:
```
crontab -e
```
Add the Task,such as(Update on 4:00am every 2 days)
```
# m h  dom mon dow   command
0 4 */2 * * bash /usr/lib/TLUpdate.sh
```

4. (Optional) Get/Discard __crontab log__

Get:
```
apt install mailutils
```

Discard:
```
apt purge mailutils
```
