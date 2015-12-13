# kutil
Chef knife utility script. Simple script to help to utilize the power of the chef index in daily work.

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
Usage:    kutil <OPTION> <VAR>
Where:    <OPTION>, see below
          <VAR>	 = Variable input (=string or part of it)
Options:  -f, -fj  = FQDN, -fj in JSON format
          -n, -nj  = Node name, -nj in JSON format
          -e, -ej  = Environment, -ej in JSON format
          -rl, -rlj  = Run_list, -rj in JSON format
          -ro, -roj  = Role, -rj in JSON format
          -re      = FQDN, show resources from the node
          -el      = Search for an environment
          -s, -sj  = Oracle SID, -sj in JSON format
          -so      = Oracle SID with OHAI time
          -sl      = Oracle SID, long output
          -i, -ij  = IP address, -ij in JSON format
          -cs      = Connect to the Oracle SID host with ssh
          -cn      = Connect to the node with ssh
          -st      = Knife status, status of the nodes
          -sh      = Knife status -H, nodes which are not updating to chef-server
          -h       = Print usage
          -v       = Print version
```
