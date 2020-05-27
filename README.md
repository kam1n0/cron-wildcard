# cron-wildcard

*Credit to Tib3rius* | https://tryhackme.com/room/linuxprivesc

* When a cron job script has a tar command being run with a wildcard (\*), this can be exploited.

[![Image of compress](https://github.com/kam1n0/cron-wildcard/blob/master/tmp_upload/compress.png)](#)

* Consulting GTFOBins for 'tar', there is a feature that allows other commands to be run as part of a checkpoint feature:

[![Image of gtfobins](https://github.com/kam1n0/cron-wildcard/blob/master/tmp_upload/gtfobins.png)](#)

1) Use msfvenom to generate a reverse shell ELF binary:

[![Image of msfvenom](https://github.com/kam1n0/cron-wildcard/blob/master/tmp_upload/msfvenom.png)](#)

2) Start Python server:

[![Image of pyserver](https://github.com/kam1n0/cron-wildcard/blob/master/tmp_upload/pyserver.png)](#)

3) Download shell.elf on the target machine:

[![Image of wget](https://github.com/kam1n0/cron-wildcard/blob/master/tmp_upload/wget.png)](#)

4) Make shell.elf executable

[![Image of chmod](https://github.com/kam1n0/cron-wildcard/blob/master/tmp_upload/chmod.png)](#)

5) Create these two files in /home/user:

[![Image of checkpoint](https://github.com/kam1n0/cron-wildcard/blob/master/tmp_upload/checkpoint.png)](#)

6) Start Netcat listener

[![Image of nc_nlvp](https://github.com/kam1n0/cron-wildcard/blob/master/tmp_upload/nc_nlvp.png)](#)
