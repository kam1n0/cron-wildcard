# cron-wildcard

*Credit to Tib3rius* | https://tryhackme.com/room/linuxprivesc

* When a cron job script has a tar command being run with a wildcard (\*), this can be exploited.

link compress

* Consulting GTFOBins for 'tar', there is a feature that allows other commands to be run as part of a checkpoint feature:

link gtfobins

1) Use msfvenom to generate a reverse shell ELF binary:

link msfvenom

2) Start Python server:

link pyserver

3) Download shell.elf on the target machine:

link wget

4) Make shell.elf executable

link chmod

5) Create these two files in /home/user:

link checkpoint

6) Start Netcat listener

link nc_nlvp
