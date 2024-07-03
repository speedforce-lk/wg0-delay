# wg0-delay
Bring up (activate) interface delayed
```
nano /etc/rc.local
```

add this line 
```
sh /etc/ifup_delayed.sh &
exit 0
```

and create this file for bash script 
```
nano /etc/ifup_delayed.sh
```

add this lines 
```
#!/bin/sh
sleep 60
ifup wg0
```
