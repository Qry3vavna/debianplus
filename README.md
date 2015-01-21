#debianplus
=======
<pre>
      _      _     _                     
     | |    | |   (_)                _   
   __| | ___| |__  _  __ _ _ __    _| |_ 
  / _` |/ _ \ '_ \| |/ _` | '_ \  |_   _|
 | (_| |  __/ |_) | | (_| | | | |   |_|  
  \__,_|\___|_.__/|_|\__,_|_| |_|        
                                         
                                         
v0.1 JAN2015 ::Qry3v@vna~*
</pre>
Collection of scripts and aliases for my convenience to type less and do more.

###USAGE:
append to your .bashrc
`cat aliases >>~/.bashrc`

###ALIASES:
`get`
>Shortcut for apt-get install -y, to quickly install given tool
>Usage: `get tool`

`update`
>Shortcut for apt-get update -y && apt-get upgrade -y

`cls`
>Shortcut for clear (though CTRL+L is even less typing)

`bounce`
>Shortcut for ifdown interface && ifup interface
>Interface has to be defined in /etc/network/interfaces
>Usage: `bounce interface`
>Example: `bounce eth0`

`p`
>Shortcut for ps -ef, but also allows for cascading greps
>Usage: `p`             Same as ps -ef
>Usage: `p pts`         Same as ps -ef | grep -i pts | grep -v grep
>Usage: `p pts bash`    Same as ps -ef | grep -i pts | grep -i bash | grep -v grep

`search`
>Search for tools in your repos by keywords
>Shortcut for apt-cache search tool with cascading greps
>Usage: `search nmap`         Shows packages referencing nmap
>Usage: `search nmap python`  Same as apt-cache search nmap | grep -i python

`show`
>Search for tools installed by keyword, if installed shows its info
>Shortcut for aptitude show tool and dpkg -L tool
>Usage: `show iptables`
