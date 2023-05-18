#!/bin/bash
# Declare a dictionary.
declare -A Host
Host=( [node1]='10.1.1.11' [node2]='10.1.1.12' [node3]='10.1.1.13' [node4]='10.1.1.14' )

# Traversing dictionary values.1
for node_ip in ${Host[@]};
do
  echo "One IP of these hosts is ${node_ip} .";
done

declare -A Test
Test=(
	[jsnu]='admin.jsnu.cn'
	[jsjz]='admin.jsjz.cn'
)
echo ${Test[jsjz]}
echo ${Test[jsnu]}

