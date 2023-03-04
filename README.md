# R620-Fan-Management
Script to set fan mode to manual and set fan speed to a acceptable volume. 

```
#Sets Manual Mode
ipmitool -I lanplus -H 192.168.1.186 -U root -P calvin raw 0x30 0x30 0x01 0x00

#Sets fan speed to 20%
ipmitool -I lanplus -H 192.168.1.186 -U root -P calvin raw 0x30 0x30 0x02 0xff 0x14
```
