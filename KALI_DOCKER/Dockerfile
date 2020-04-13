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
metasploit-framework \
ldapsearch \ 
enum4linux \ 
responder \
smbclient \
smbmap \
smbmount \
bloodhound \
libssl-dev \
libffi-dev \
python-dev \
build-essential \
rpcclient \



# ngrok
RUN curl https://bin.equinox.io/c/4VmDzA7iaHb/ngrok-stable-linux-amd64.zip | gunzip - > /usr/bin/ngrok && \
    chmod +x /usr/bin/ngrok
# crackmapexec
RUN git clone --recursive https://github.com/byt3bl33d3r/CrackMapExec

# impacket
RUN git clone https://github.com/SecureAuthCorp/impacket.git

# mimikatz
git clone https://github.com/gentilkiwi/mimikatz.git

# ranger
RUN wget https://raw.githubusercontent.com/funkandwagnalls/ranger/master/setup.sh && chmod a+x setup.sh && ./setup.sh && rm setup.sh

# powersploit
RUN git clone https://github.com/PowerShellMafia/PowerSploit.git

# evil-winRm
RUN git clone https://github.com/Hackplayers/evil-winrm.git && cd evil-winrm && gem install evil-winrm
