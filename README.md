git clone https://github.com/UluBeyCRS/DDOS-TOOL.git

# Kali linux:
sudo apt update && sudo apt upgrade -y
sudo apt install python3 python3-pip -y
sudo apt install python3-scapy -y
pip3 install requests colorama netifaces
sudo python3 ddos2.0.py

# Termux:
pkg update && pkg upgrade -y
pkg install python python-pip -y
pkg install python-scapy -y
pip install requests colorama netifaces
su -c "python3 stormbreaker.py"
python3 stormbreaker.py
