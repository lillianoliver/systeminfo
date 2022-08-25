#!/bin/bash
####System inventory script by Lillian

echo -n "Name"
uname -n
echo -n "IP"
ifconfig | grep inet adress
echo -n "CPU"
lscpu
echo -n "OS"
uname -r
echo -n "Memory"
free -m
echo -n "Runtime"
top
echo -n "32 or 64 bits"
getconf LONG_BIT
echo -n "Block devices"
lsblk
echo -n "Processing units" 
nproc
echo "Up for"
uptime
        