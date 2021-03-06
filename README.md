# kutil
Chef knife utility script. Simple bash script to help to utilize the power of the chef index in your daily work. Finding information is normally behind lengthy knife search commands. kutil helps to shorten the effort and give a "toolbox" to get information fast. Additionally kutil works nicely for Oracle databases environments, if you use the https://github.com/aririikonen/oracle cookbook. For example with:

```
kutil -cs <SID>
```

You can easily login with ssh to databases using the database name instead of trying to figure out which FQDN the database has.

# Setup
Change the CHEF_HOME variable to match your chef repo home.

```
...
CHEF_HOME=~/chef
...
```

# Usage
```
kutil 1.0.3 3.12.2015
Usage:    kutil <option> <search_string>
Where:    <option>            = See options below
          <search_string>	= Search string (or part of it)
Options:  -f, -fj    = FQDN, -fj in JSON format
          -n, -nj    = Node name, -nj in JSON format
          -e, -ej    = Environment, -ej in JSON format
          -rl, -rlj  = Run_list, -rj in JSON format
          -ro, -roj  = Role, -rj in JSON format
          -re        = FQDN, show resources from the node
          -el        = Search for an environment
          -s, -sj    = Oracle SID, -sj in JSON format
          -so        = Oracle SID with OHAI time
          -sl        = Oracle SID, long output
          -i, -ij    = IP address, -ij in JSON format
          -cs        = Connect to the Oracle SID host with ssh
          -cn        = Connect to the node with ssh
          -st        = Knife status, status of the nodes
          -sh        = Knife status -H, nodes which are not updating to chef-server
          -h         = Print usage
          -v         = Print version
```
