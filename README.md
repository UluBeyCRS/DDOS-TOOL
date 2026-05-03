git clone https://github.com/UluBeyCRS/DDOS-TOOL.git

# Kali linux:
# Update system
sudo apt update && sudo apt upgrade -y

# Install Python and pip if not installed
sudo apt install python3 python3-pip -y

# Install Scapy (requires root for raw sockets)
sudo apt install python3-scapy -y

# Install required Python libraries
pip3 install requests colorama netifaces

# Run with root privileges (required for SYN flood, ICMP flood, IP spoofing)
sudo python3 stormbreaker.py

# Termux:
# Update Termux
pkg update && pkg upgrade -y

# Install Python and dependencies
pkg install python python-pip -y

# Install Scapy and dependencies
pkg install python-scapy -y

# Install required Python libraries
pip install requests colorama netifaces

# Termux requires root for raw sockets (ICMP flood, SYN flood)
# If device is rooted:
su -c "python3 stormbreaker.py"

# If NOT rooted: run without sudo (HTTP flood, Slowloris, SSL flood will work)
python3 stormbreaker.py
