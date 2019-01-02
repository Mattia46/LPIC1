## Proc filesystem (/proc) - not persistent

Is created in RAM at boot time, so overridden every boot
Only Root can change the proc filesystem

es: /proc/sys/fs has a *file-max* that specify the max number of file you can open at the same time.
If you change it echo 10000 > /proc/sys/fs/file-max as a Root it will be override to the original
value at the next boot.

