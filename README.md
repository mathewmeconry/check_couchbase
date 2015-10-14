# check_couchbase 
Icinga plugin to check couchbase cluster 
<br><br>
## Requirements
The package jq is needed to parse the responses of the api<br>
<br>
For Example:<br>
 apt-get install jq
<br><br>
## Parameters
    -cc / --check-cluster   Checks the connection between this node and the others (-w = warninig hosts down / -c = critical hosts down) <br>
    -cn / --check-node      Checks this node which different performace data (-c and -w not in use) <br>
    -u / --user             Login username <br>
    -p / --passsword        Login password <br>
    -P / --port             API port <br>
    -h / --host             IP address <br>
    -w / --warning          Warning value (only with --check-cluster in use) default: 0 <br>
    -c / --critical         Critical value (only with --check-clsuter in use) default: 0 <br>
<br><br>
## Returns
### check-cluster (-cc)<br>
    Returns count of healthy and failed hosts 

### check-node (-cn)<br>
    Returns state,ram used, cpu utilization, swap used, current items and uptime as performance data 
    
## Feature requests
Please send feature requests to this repository
