### List bound local ports
`sudo netstat -tulpn | tail -n +3 | awk -F '[[:space:]]+' '{print $4}' | awk -F ':' '{print $NF}' | sort`
