# zabbix_template_tcp

TCP Connection Status Template for Zabbix ~> 3.4.

Necessary "Dependent Item". Put userparameter_tcp.conf in Include-UserParameter's Directory and Put json_item_tcp.sh in /var/lib/zabbix .

- TCP Connection Status Template for Zabbix 3.4.
- It was a bit too complicated to do ... with the UserParameter wine liner so we got JSON across the wrapper script and put it in the dependent item.
- It is the default for CentOS. Please use bash with FreeBSD and use json_item_tcp.sh.freebsd.
- Since Linux counts up from the proc file system, you do not need to include net-tools. That netstat is slow so it will take more than 5 seconds on a 5 digit connection and will time out.
- I thought about calculating UNKNOWN but it is 0 so far so it's troublesome.

This template is MIT License.
