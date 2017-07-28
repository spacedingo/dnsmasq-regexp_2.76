### Dnsmasq version 2.76 - with regex and extended cache limit
Added regex matching support for use with `address` and extended maximum cache limit from 10,000 to 500,000.

------------
##### Example config

Regex matching `address=/:myvpn[0-9].company.com:/4.1.1.1`

More cache `cache-size=300000`

------------


##### Compiling (Debian 8/9 or Ubuntu 16/17)
###### 1. Install prerequisites:
    apt-get install -y git make gcc libdbus-1-dev libidn11-dev libnetfilter-conntrack-dev liblua5.1-dev libpcre++-dev nettle-dev libhogweed4
###### 2. Compile:
    git clone https://github.com/spacedingo/dnsmasq-regexp_2.76.git dnsmasq
    cd dnsmasq
    make install


------------


##### Links
###### [Dnsmasq-discuss] using regular expressions in server list
http://lists.thekelleys.org.uk/pipermail/dnsmasq-discuss/2013q2/007124.html
###### dnsmasq-2.63-regex.patch
http://lists.thekelleys.org.uk/pipermail/dnsmasq-discuss/attachments/20130428/b3fc0de0/attachment.obj
###### Compiling dnsmasq 2.76
https://forums.fogproject.org/topic/8725/compiling-dnsmasq-2-76-if-you-need-uefi-support/6
###### [Dnsmasq-discuss] why limit cache size to 10000?
http://lists.thekelleys.org.uk/pipermail/dnsmasq-discuss/2007q4/001650.html
