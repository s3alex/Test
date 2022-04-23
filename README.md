-#!/bin/bash
#Author: Alex
#Date: 04/21/22
#The purpose of this script is to check the swap memory

uname=`uname -a |awk -F"#" '{print$2}' |awk -F "-" '{print$2}'|awk '{print $1}'`
if [[ $uname=Linux ]]
then
echo "we are good the kernal name is $uname"

else
echo "we are not good"
fi
