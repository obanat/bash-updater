# YDNS Bash Updater Script

This repository contains the bash updater script which can be used on *NIX-like environments to update dynamic hosts. It is recommended to use this script with cronjob to run periodically (preferrably every 15 minutes).

The script uses the YDNS API v1 (dyn-compatible).

## usage

Available options are:
  -h             Display usage
  -H HOST        YDNS host to update
  -u USERNAME    YDNS username for authentication
  -p PASSWORD    YDNS password for authentication
  -i INTERFACE   Use the local IP address for the given interface
  -v             Display version
  -V             Enable verbose output
  -4             use ipv4   (new add)
  -6             use ipv6   (new add)
