# Linux Cheatsheet 

## Find files larger than given size (gb/mb/kb/bytes) 
```
find / -type f -size +100M -exec ls -lh {} \; | awk '{ print $9 "|| Size : " $5 }'
```
