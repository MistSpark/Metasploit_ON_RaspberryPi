# How to Install Metasploit On RaspberryPi

Of course you can install Kali Linux on RaspberryPi, but I didn't do that, I don't use my RaspberryPi for hacking, but at some point I needed Metasploit Framework, so I had to install it.

This is how I did it:

00- apt update && apt upgrade

01- apt -y install build-essential zlib1g zlib1g-dev libxml2 libxml2-dev libxslt-dev locate libreadline6-dev libcurl4-openssl-dev git-core libssl-dev libyaml-dev openssl autoconf libtool ncurses-dev bison curl wget postgresql postgresql-contrib libpq-dev libapr1 libaprutil1 libsvn1 libpcap-dev

02- apt install ruby-dev

03- cd /opt

04- git clone https://github.com/rapid7/metasploit-framework.git

05- cd metasploit-framework

06- apt install git-core postgresql curl ruby1.9.3 nmap gem

07- gem install wirble sqlite3 bundler

08- gem install nokogiri 

09- gem install bundle

10- bundle install

11- ./msfconsole
