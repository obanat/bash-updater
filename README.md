# YDNS Bash Updater Script

This repository contains the bash updater script which can be used on *NIX-like environments to update dynamic hosts. It is recommended to use this script with cronjob to run periodically (preferrably every 15 minutes).

The script uses the YDNS API v1 (dyn-compatible).

## usage

Available options are:

  -f             Specify ipv6 perfix

  -h             Display usage
  
  -H HOST        YDNS host to update
  
  -u USERNAME    YDNS username for authentication
  
  -p PASSWORD    YDNS password for authentication
  
  -i INTERFACE   Use the local IP address for the given interface
  
  -v             Display version
  
  -V             Enable verbose output
  



## 说明
增加了-f 参数，用于指定过滤的ipv6前缀，用法

./update.sh -f 2409* -i pppoe-wan -V

上述脚本会将pppoe-wan接口中匹配2409开头的ipv6地址，更新到服务器上
