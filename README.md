# How to Install Metasploit On RaspberryPi

While it's possible to install Kali Linux on a Raspberry Pi, I haven't done so myself. I don't use my Raspberry Pi for hacking purposes. However, there was a situation where I needed the Metasploit Framework, so I had to install it. Here's how I went about it:

00- apt update && apt upgrade

01- apt -y install build-essential zlib1g zlib1g-dev libxml2 libxml2-dev libxslt-dev locate libreadline6-dev libcurl4-openssl-dev git-core libssl-dev libyaml-dev openssl autoconf libtool ncurses-dev bison curl wget postgresql postgresql-contrib libpq-dev libapr1 libaprutil1 libsvn1 libpcap-dev

02- apt install ruby-dev

03- cd /opt

04- git clone https://github.com/rapid7/metasploit-framework.git

05- cd metasploit-framework

06- apt install git-core postgresql curl nmap gem libsqlite3-dev

07- gem install wirble sqlite3 bundler

08- gem install nokogiri 

09- gem install bundle

10- bundle install

11- ./msfconsole
