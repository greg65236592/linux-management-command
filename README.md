# linux-management-command
frequent used linux commands

### List disk space
df -h

### List directory space (sort by size)
du -sh * | sort -h

### List file details
ls -l

### Too many open files exam
lsof > ~/Desktop/lsof.log

cat ~/Desktop/lsof.log | awk '{ print $2 " " $1; }' | sort -rn | uniq -c | sort -rn | head -20

vim ~/Desktop/lsof.log

### process monitor
top


