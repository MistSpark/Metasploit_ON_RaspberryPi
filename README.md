# How to Install Metasploit On RaspberryPi

Of course you can install Kali Linux on RaspberryPi, but I didn't do that, I don't use my RaspberryPi for hacking, but at some point I needed Metasploit Framework, so I had to install it.

This is how I did it:

0- apt update && apt upgrade

1- apt-get -y install build-essential zlib1g zlib1g-dev libxml2 libxml2-dev libxslt-dev locate libreadline6-dev libcurl4-openssl-dev git-core libssl-dev libyaml-dev openssl autoconf libtool ncurses-dev bison curl wget postgresql postgresql-contrib libpq-dev libapr1 libaprutil1 libsvn1 libpcap-dev

2- apt install ruby-dev

3- cd /opt

4- git clone https://github.com/rapid7/metasploit-framework.git

5- cd metasploit-framework

6- gem install nokogiri 

7- gem install bundle

8- bundle install

9- ./msfconsole
