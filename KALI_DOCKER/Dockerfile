FROM kalilinux/kali-rolling

# source list
RUN echo "deb http://archive-7.kali.org/kali kali-rolling main contrib non-free" > /etc/apt/sources.list && \
    echo "deb-src http://archive-7.kali.org/kali kali-rolling main contrib non-free" >> /etc/apt/sources.list && \
    echo "deb http://http.kali.org/kali kali-rolling main non-free contrib" > /etc/apt/sources.list

RUN apt-get -y update && apt-get -y dist-upgrade && apt-get -y autoremove && apt-get clean

# tools
RUN apt-get install -y \
git \
unzip \
nano \
tmux \ 
curl \
telnet \
strace \
ltrace \
wget \
net-tools \
python \
python3 \
python3-pip \
sslscan \
wordlists \
wfuzz \
gobuster \
hashcat \
gdb \
dnsmap \
ftp \
knocker \
nmap \
sqlmap \
seclists \
powersploit \
smbmap \
unicornscan \
masscan \
tcpdump \
ncat \
openvpn \
metasploit-framework 


# ngrok
RUN curl https://bin.equinox.io/c/4VmDzA7iaHb/ngrok-stable-linux-amd64.zip | gunzip - > /usr/bin/ngrok && \
    chmod +x /usr/bin/ngrok
