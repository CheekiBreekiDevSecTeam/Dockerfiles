FROM kalilinux/kali-linux-docker:latest


# Install Kali Full
RUN apt-get clean && \
    apt-get update -y && \
    apt-get install -y software-properties-common kali-linux-full --fix-missing

RUN echo "deb http://archive-7.kali.org/kali kali-rolling main contrib non-free" > /etc/apt/sources.list && \
    echo "deb-src http://archive-7.kali.org/kali kali-rolling main contrib non-free" >> /etc/apt/sources.list

# tools
RUN apt-get install -y git unzip nano tmux curl telnet strace ltrace less wget net-tools  python python3 \
python-pip python3-pip sslscan wordlists wfuzz gobuster hashcat gdb dnsmap ftp knocker nmap sqlmap seclists \
powersploit smbmap unicornscan masscan tcpdump ncat openvpn metasploit-framework 


# ngrok
RUN curl https://bin.equinox.io/c/4VmDzA7iaHb/ngrok-stable-linux-amd64.zip | gunzip - > /usr/bin/ngrok && \
    chmod +x /usr/bin/ngrok
